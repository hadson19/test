# test
test github feature
The above schema defines the following constraints:
* `schoolRun`
    * type: `boolean`
    * default: `true`
* `minimumVersion`
    * type: `string`
    * default: `2.0.0`
* `chatBotChat`
    * type: `boolean`
    * default: `true`
* `chatBotCall`:
    * type: `boolean`
    * default: `true`
* `autoPlayDelay`:
    * type: `number`
    * default: 3000,

* `helpLink`:
    * type: `string`
    * format: `uri`
    * default: `https://www.dpd.co.uk/lp/app/index.html`

* `banners`:
    * type: array
    * item: 
        * `image`:
          * one of the following: 
              * type: `string`, format: `uri`
              * type:`number`
          * required

        * `advertiserId`:
          * type: `string`  
          * required: `true`

        * `title`:
          * type: `string`  
          * required: `true`

    * default: <details> <summary>array</summary>
        ```ts
      [
          {
            "image": "https://www.dpdgroup.co.uk/ShipBanner.png",
            "actionType": "ship"
          },
          {
            "image": "https://www.dpdgroup.co.uk/UKShoppingDsicounts.png",
            "actionType": "partner_rewards"
          },
          {
            "image": "https://www.dpdgroup.co.uk/DSBanner.png",
            "actionType": "design_space"
          },
          {
            "video": "https://firebasestorage.googleapis.com/v0/b/dpduk-p-yourdpd-d4.appspot.com/o/static%2Fbanners%2Fwestminster_depot_opening%2Fvideo.mp4?alt=media&token=f39d7b15-3a5f-4540-9d09-d50990383059",
            "image": "https://www.dpdgroup.co.uk/NewsBanner.png",
            "actionType": "video"
          }
      ]
      ```
      </details>
    
* `birthyear`
    * an integer between 1900 and 2013
    * <details><summary>default</summary>
        ```ts
        [
          {
            "image": "https://www.dpdgroup.co.uk/ShipBanner.png",
            "actionType": "ship"
          },
          {
            "image": "https://www.dpdgroup.co.uk/UKShoppingDsicounts.png",
            "actionType": "partner_rewards"
          },
          {
            "image": "https://www.dpdgroup.co.uk/DSBanner.png",
            "actionType": "design_space"
          },
          {
            "video": "https://firebasestorage.googleapis.com/v0/b/dpduk-p-yourdpd-d4.appspot.com/o/static%2Fbanners%2Fwestminster_depot_opening%2Fvideo.mp4?alt=media&token=f39d7b15-3a5f-4540-9d09-d50990383059",
            "image": "https://www.dpdgroup.co.uk/NewsBanner.png",
            "actionType": "video"
          }
        ]
        ```
        </details>


* `email`
    * a valid email address string
    * must have two domain parts e.g. `example.com`

