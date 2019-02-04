# Remote config validation

* `schoolRun`
    * type: `boolean`
    * `default`    `true`
    

* `minimumVersion`
    * type: `string`
    * `default`    `2.0.0`
    

* `chatBotChat`
    * type: `boolean`
    * `default`    `true`
    

* `chatBotCall`
    * type: `boolean`
    * `default`    `true`
    

* `autoPlayDelay`
    * type: `number`
    * `default`    `3000`
    
    * the next values cannot be used: `Infinity`, `-Infinity`

* `helpLink`
    * type: `string`
    * `default`    `https://www.dpd.co.uk/lp/app/index.html`
    

* `banners`
    * type: `array`
    * `default`<details><summary>expand</summary>
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
    
    * items: 
        * `image`
            * one of the next item should be used: 
                * item 1
                    * type: `string`
                    * `uri`
                * item 2
                    * type: `number`
                    * the next values cannot be used: `Infinity`, `-Infinity`
            * `required`
        
        * `video`
            * type: `string`
            * `uri`
        
        * `actionType`
            * type: `string`
            * only the next values can be used: `video`, `design_space`, `ship`, `partner_rewards`
        
        

* `partnerLogos`
    * type: `array`
    * `default`<details><summary>expand</summary>
        ```ts
        [
          {
            "image": "https://www.dpdgroup.co.uk/Asos.png",
            "advertiserId": "5678",
            "title": "Asos"
          },
          {
            "image": "https://www.dpdgroup.co.uk/Nike.png",
            "advertiserId": "6373",
            "title": "NIKE UK"
          },
          {
            "image": "https://www.dpdgroup.co.uk/EE_logo.png",
            "advertiserId": "5571",
            "title": "EE Mobile"
          },
          {
            "image": "https://www.dpdgroup.co.uk/PCWorld.png",
            "advertiserId": "1599",
            "title": "Currys PC World"
          },
          {
            "image": "https://www.dpdgroup.co.uk/Topshop.png",
            "advertiserId": "6009",
            "title": "Topshop UK"
          },
          {
            "image": "https://www.dpdgroup.co.uk/Topman.png",
            "advertiserId": "2479",
            "title": "Topman UK"
          }
        ]
        ```
    </details>
    
    * items: 
        * `image`
            * one of the next item should be used: 
                * item 1
                    * type: `string`
                    * `uri`
                * item 2
                    * type: `number`
                    * the next values cannot be used: `Infinity`, `-Infinity`
            * `required`
        
        * `advertiserId`
            * type: `string`
            * `required`
        
        * `title`
            * type: `string`
            * `required`
        
        

* `prohibitedDescription`
    * type: `array`
    * `default`<details><summary>expand</summary>
        ```ts
        [
          {
            "type": "text",
            "source": [
              "THE FOLLOWING ITEMS (OR ANY ITEM SIMILAR IN DESCRIPTION OR CONTENT) CAN NOT BE CARRIED ON ANY SERVICE.",
              "Any person sending such an item may be subject to their order being cancelled without notice:"
            ]
          },
          {
            "type": "list",
            "source": [
              "Active Mobile Phones Outside The EU",
              "Aerosol",
              "Aftershaves",
              "Air Bag",
              "Alcoholic Beverages",
              "Amber",
              "Ammunition",
              "Animals Or Organisms Of Any Form (Alive Or Dead)",
              "Any Articles (Or Part Of Them) That Are Made Up Of China, Glass, Porcelain, Earthenware Or Other Similar Materials",
              "Any Item Containing Petrol (Liquid, Gas Or Fumes)",
              "Aromatherapy Oil",
              "Art",
              "Basins",
              "Batteries",
              "Beds & Headboards",
              "Biological Samples",
              "Birds",
              "Boiler/Boilers",
              "Bottles",
              "Bulbs",
              "Camera",
              "Camping Gas All Types",
              "Canvas Print",
              "Car Panel",
              "Cash, Credit Cards, Debit Cards",
              "Ceramics/Figures/Figurines",
              "Chainsaw",
              "Cheques",
              "China/Porcelain",
              "Chocolate",
              "Christmas Crackers",
              "Clock",
              "Coffee Machines",
              "Computer Monitor/Monitors/Imac",
              "Concrete",
              "Confectionery",
              "Counterfeit Currency",
              "Credit/Debit/Cash Cards",
              "Crockery/Pots/Pottery",
              "Crystal",
              "Dangerous Goods",
              "Delicate Items",
              "Detergent",
              "Diamonds",
              "Documents",
              "Domestic Appliances (Washing Machines, Dryers, Fridges, Ovens)",
              "Driving Licence",
              "Drugs (Including Prescription)",
              "Engines",
              "Fiberglass",
              "Fire Crackers",
              "Fire Extinguisher",
              "Firearms",
              "Fireworks",
              "Fish (Live Or Dead)",
              "Fish Tank",
              "Fishing Rods",
              "Flammable Goods",
              "Food Items",
              "Fragile Items (All)",
              "Fragrance",
              "Framed Painting/Photograph",
              "Furniture (Including Flat-Packed)",
              "Furs",
              "Gearbox",
              "Gems Or Gemstones",
              "Glass/Glassware",
              "Granite Products",
              "Hamper",
              "Hazardous Goods",
              "Hover Board/Swegway/Segway",
              "Human Flesh",
              "Human Remains",
              "Infectious Substances",
              "Item Described As \"Unknown\"",
              "Ivory",
              "Jewellery Including Watches",
              "Juice",
              "Kayaks",
              "Knives",
              "Ladders",
              "Lampshades",
              "Legal Or Business Documents",
              "Lenses",
              "Lighter",
              "Lights/Lighting/Lamps/Chandeliers",
              "Liquids/Creams/Oils",
              "Lottery Tickets",
              "Machines",
              "Magnets",
              "Marble Products",
              "Mattresses",
              "Meat",
              "Medical Equipment",
              "Microscope",
              "Microwave",
              "Milk Powder (Formula)",
              "Mirror",
              "Mobile Phone/Mobile Phones With Or Without Sim To Any Address In Turkey/Pakistan/Ecuador",
              "Money/Cash/Currency/Vouchers",
              "Nail Varnish",
              "Oil",
              "Ornament",
              "Over Head Projector",
              "Packaging/Media Packaging",
              "Paint",
              "Painting/Pictures",
              "Passport",
              "Perfumes",
              "Perishable Goods (All)",
              "Personal Items",
              "Petrol Or Diesel Tanks (Full Or Empty) In Any Item",
              "Pewter Figures",
              "Picture Frames",
              "Plant/S",
              "Poster",
              "Precious Metals (Gold/Silver/Platinum Etc.)",
              "Print",
              "Printer Toner/ Ink Cartridges",
              "Projector",
              "Real Fur",
              "Replica Weapons",
              "Resin",
              "Scanner",
              "Seatbelt Tensioner",
              "Settee",
              "Sewing/Knitting Machine",
              "Shower Screen",
              "SIM Cards",
              "Slush Syrup",
              "Slush Syrup",
              "Sofa",
              "Spectacles",
              "Stamps (Unless Franked)",
              "Steering Wheel",
              "Stoneware",
              "Suitcases/ Flight Cases (Not Acceptable As Packaging)",
              "Surf Board",
              "Telescope",
              "Television",
              "Tickets",
              "Tiles",
              "Tobacco And Tobacco Products",
              "Toilets",
              "Torches",
              "Trees",
              "Turntables",
              "Tyres",
              "Vase",
              "Vehicle Bonnet",
              "Vehicle Bumper",
              "Vehicle Door",
              "Velux",
              "Vermiculite Board",
              "Vouchers With A Face Value",
              "Watch",
              "Water",
              "Weapons",
              "Wheels",
              "Window",
              "Window Frame",
              "Wooden Items (Australia)"
            ]
          },
          {
            "type": "text",
            "source": [
              "SPECIAL PROVISIONS:"
            ]
          },
          {
            "type": "list",
            "source": [
              "Amplifiers - maximum parcel compensation value for damages is £200, up to £2,500 compensation for lost items.",
              "Apple Mac - maximum parcel compensation value for damages is £200, up to £2,500 compensation for lost items. iMacs are covered for loss only",
              "Banjo - maximum parcel compensation value for damages is £100, up to £1,000 compensation for lost items. Banjo must be sent in a hard case.",
              "Cello - maximum parcel compensation value for damages is £100, up to £1,000 compensation for lost items. Cello must be sent in a hard case.",
              "Guitar - maximum parcel compensation value for damages is £100, up to £1,000 compensation for lost items. Guitar must be sent in a hard case.",
              "Macpro - maximum parcel compensation value for damages is £200, up to £2,500 compensation for lost items. iMacs are covered for loss only",
              "Violin - maximum parcel compensation value for damages is £100, up to £1,000 compensation for lost items. Violin must be sent in a hard case."
            ]
          }
        ]
        ```
    </details>
    
    * items: 
        * `type`
            * type: `string`
            * `required`
            * only the next values can be used: `text`, `list`
        
        * `source`
            * type: `array`
            * `required`
            * items: 
                * type: `string`
                
        
        

* `advertiserLogosMapping`
    * type: `object`
    * `default`<details><summary>expand</summary>
        ```ts
        {
          "2487": "https://www.dpdgroup.co.uk/logos/customer-maint-notification-341173.png",
          "4182": "http://31cd35098195e2510dc4-37bc6a2097e4b87eca67bfae231c19f8.r16.cf3.rackcdn.com/customer-maint-notification-451460-13.jpg",
          "6373": "http://31cd35098195e2510dc4-37bc6a2097e4b87eca67bfae231c19f8.r16.cf3.rackcdn.com/customer-maint-notification-302868-6.png"
        }
        ```
    </details>
    
    * The key of object is dynamic and should be valid to the next rules:
        * prop regex: `/\s*/`
        * value: 
            * type: `string`
            * `uri`
