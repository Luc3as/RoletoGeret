# Roleto Geret
Smart motorised roller shades, heavily inspired by this design, https://www.thingiverse.com/thing:2392856

I know there are many projects like this, however I took slightly different approach by making this device self powered by solar panel, and with implemented reed switch to act as hardware endstop. 

## Bill of material
* [Roller shade](merkurymarket.sk/vrobok/roleta-na-stenu-180x175-k835,85523.html) (Choose the right size and color for you)
* [Wemos D1 mini](http://s.click.aliexpress.com/e/b7xoMFF6) 
* [Bearings 8x16x5](https://www.aliexpress.com/item/32857798603.html?spm=a2g0o.productlist.0.0.54fb223eH3GoX2&algo_pvid=5aeb96ee-0202-4036-b42f-7ed2e9f3ded6&algo_expid=5aeb96ee-0202-4036-b42f-7ed2e9f3ded6-1&btsid=0bb0623316159863064161308ec46b&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
* [Plastic reed switch](https://www.aliexpress.com/item/32725119865.html?spm=a2g0o.productlist.0.0.ffd16b03I2m48r&algo_pvid=d63ebcdd-0437-4bf0-9498-7caa7aee1411&algo_expid=d63ebcdd-0437-4bf0-9498-7caa7aee1411-7&btsid=0bb0623316159863660961735ec46b&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
* [28BYJ-48 motor with ULN2003 driver](https://www.aliexpress.com/item/33011650711.html?spm=a2g0o.productlist.0.0.538c6e6aDcBTwc&algo_pvid=c6948097-cef4-4100-a6a4-3a148faee855&algo_expid=c6948097-cef4-4100-a6a4-3a148faee855-38&btsid=0bb0623a16159864338042717ec4c9&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)  (Buy the longer and slimmer driver version of ULN2003)
* [Tactile push buttons](http://s.click.aliexpress.com/e/0rbMNuk)
* [Resistors](http://s.click.aliexpress.com/e/boawi0Ak)
* [18650 battery](https://www.aliexpress.com/item/4001139242149.html?spm=a2g0o.productlist.0.0.2c1f42b3OON2Uh&algo_pvid=873851fa-bf57-4310-a192-b8a27ef4debc&algo_expid=873851fa-bf57-4310-a192-b8a27ef4debc-0&btsid=0b0a555716159866024315992e1132&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_) (I harvested mine from old laptop battery)
* [TP4056 LiPo charger](https://www.aliexpress.com/item/1005001636470790.html?spm=a2g0o.productlist.0.0.7ef163cbWSA0sV&algo_pvid=null&algo_expid=null&btsid=0bb0623216159866494856204eb2d0&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
* [DC-DC boost converter](aliexpress.com/item/4000283425849.html?spm=a2g0s.9042311.0.0.3bb24c4d8f2NIH)
* [Solar panel](https://www.aliexpress.com/item/33047177046.html?spm=a2g0s.9042311.0.0.3bb24c4d8f2NIH)
* Some basic soldering equipment and skills

## Wiring scheme
![Wiring scheme](/Images/roletogeret_bb.png)

## Firmware
As always, I used ESPHome as firware of choice, I found great piece of code somewhere on forum of HomeAssistant. I modified the code to accept the physical end stop through reed switch, and also modified behaviour of physical push button on controller, now it acts as Close/Stop/Open so you can adjust the desired height through button.

## Physical installation
Device is mounted to wall by self adhesive tape by 3M.

For cable routing I used sticky cable trunking with name MONTERA. 
For fully closing/opening this approximately 160cm roller takes about 5 minutes, which is actually fine for me, because I use the slowly comming light to gently waking me up. Motor and all mechanics are very quiet for my surprise, I think bearing helped a lot. 

Also you can choose the side of mounting the motor, I mirrored all parts to both sides. You can swap PIN order in ESPHome config file. (See Stepper motor definition)


All parts for 3D printing are on [thingiverse project page](https://www.thingiverse.com/thing:4783606)

![]()
![]()
![]()
![]()
![]()

### If You liked my work, You can buy me a coffee :)

<a class="" target="_blank" href="https://www.buymeacoffee.com/luc3as"><img src="https://lukasporubcan.sk/images/buymeacoffee.png" alt="Buy Me A Coffee" style="max-width: 217px !important;"></a>

### Or send some crypto

<a class="" target="_blank" href="https://lukasporubcan.sk/donate"><img src="https://lukasporubcan.sk/images/donatebitcoin.png" alt="Donate Bitcoin" style="max-width: 217px !important;"></a>	
			