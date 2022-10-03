---
layout: single
title:  "Installing a Shelly 1L & Motion sensor in the Garage"
date: 2022-10-02
categories: Computing IOT Hubitat

gallery1:
  - url: /assets/images/Garage-Room-IOT/Back_Door_Switch.jpg
    image_path: /assets/images/Garage-Room-IOT/Back_Door_Switch.jpg     
    alt: "Back Door Switch"
    title: "Back Door Switch"
  - url: /assets/images/Garage-Room-IOT/Back_Door_Switch_Wiring.jpg
    image_path: /assets/images/Garage-Room-IOT/Back_Door_Switch_Wiring.jpg
    alt: "Back Door Switch Wiring"
    title: "Back Door Switch Wiring"
  - url: /assets/images/Garage-Room-IOT/Front_Door_Switch.jpg
    image_path: /assets/images/Garage-Room-IOT/Front_Door_Switch.jpg
    alt: "Garage Door Switch"
    title: "Garage Door Switch"
  - url: /assets/images/Garage-Room-IOT/Front_Door_Switch_Wiring.jpg
    image_path: /assets/images/Garage-Room-IOT/Front_Door_Switch_Wiring.jpg
    alt: "Garage Door Switch"
    title: "Garage Door Switch"
  - url: /assets/images/Garage-Room-IOT/Philips_Hue_Motion_Sensor.jpg
    image_path: /assets/images/Garage-Room-IOT/Philips_Hue_Motion_Sensor.jpg
    alt: "Motion Sensor"
    title: "Motion Sensor"
gallery2:
  - url: /assets/images/Garage-Room-IOT/Garage_Lights.jpg
    image_path: /assets/images/Garage-Room-IOT/Garage_Lights.jpg
    alt: "Garage Lights"
    title: "Garage Lights"


---

I now have the ability to contol my garage florescent light strips by voice using my [Google Nest Mini](https://store.google.com/gb/config/google_nest_mini?hl=en-GB), or by using the [Google Home app](https://apps.apple.com/us/app/google-home/id680819774) on my phone when I'm out and about. I live in an older house so my light circuit doesn't have a neutral, for this reason I'm using the [Shelly 1L](https://shellystore.co.uk/product/Shelly-1L/). Thankfully, these Florescent lights draw 20W each, so there isn't a need for a [Shelly Bypass](https://smarthomeshopuk.com/products/shelly-bypass).

{: .notice--danger}
**Electical Danger :** Remember to switch off the circuit at the fuse box (consumer unit) and check with a meter or an electrical testing pen that the circuit is off before working on it, mains electricity can kill. If you don’t know what you're doing and/or, are not comfortable working with  mains electricity, then pay an electrician to do the work.

### Parts List

|**Part**|**Price** |
|-|-|
|Shelly [1L](https://shellystore.co.uk/product/shelly-1l/) | £17:00 |
|Philips Hue [Motion Sensor](https://amzn.eu/d/9HBs1sy)| £39:99 |
|**Total Price** | **£56:99** |

Programming the Hubitat to use Rules Machine instead of Simple Rules, as this allows me to program TTS (Text To Speech) so we know if anyone has opened the garage door from the Living Rooms Nest Hub.

### Installation Photos

{% include gallery id="gallery1" layout="third" caption="Gallery of switch wiring" %}

{% include gallery id="gallery2" layout="quarter" caption="Florescent Lights" %}
