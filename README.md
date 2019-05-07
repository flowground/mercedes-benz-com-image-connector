# ![LOGO](logo.png) Vehicle Image **flow**ground Connector

## Description

A generated **flow**ground connector for the Vehicle Image API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/mercedes-benz.com/image/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:59+03:00

## API Description

The vehicle images API offers access to original Mercedes-Benz vehicle images.  It provides access to exterior and interior images with parameters e.g. to modify the perspective and to display vehicles at day/nighttime.  In addition you can request component images of a vehicle's engine, paint, rim, trim, upholstery and equipments.

## Authorization

This API does not require authorization.

## Actions

### Returns URLs pointing to images in JPG format in the highest available resolution (depending on the component) of the vehicle's:<br/>
>   * engine (1024x576 px), <br/>
>   * rim (710x710 px), <br/>
>   * trim (800x600 px), <br/>
>   * paints (800x600 px), <br/>
>   * upholstery (800x600 px) and <br/>
>   * equipments (740x416 px).

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components

### Returns a URL pointing to an image of the vehicles engine.  These images are available in the resolution 1024x576 px.

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components_engine

### Returns URLs pointing to images of this vehicle's equipments. The images are available in the highest possible resolution (usually 740x416 px).

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components_equipments

### Returns URLs pointing to images of this vehicles paint.  These images are available in resolution 800x600 px.  Note there might be two paints (e.g. Smart, 'paint' for body panel and 'paint2' for the tridion cell)

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components_paint

### Returns a URL pointing to an image of the vehicles rim.  These images are available in the resolution 710x710 px.

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components_rim

### Returns a URL pointing to an image of this vehicles trim.  These images are available in resolution 800x600 px.

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components_trim

### Returns URLs pointing to images of the vehicle's upholsteries. Tge images are available in the highest possible resolution (usually 800x600 px).

*Tags:* `Components`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345

### x_swagger_router_controller__finorvin__components_upholstery

### Returns URLs pointing to PNG images of a vehicle with a transparent background.

*Tags:* `Perspectives`

#### Input Parameters
* `finorvin` - _required_ - The FIN or VIN of one specific vehicle. For testing purposes the following sample FINs are available (please note that these FINs are NOT available in the tryout): 
  * E 350 d: WDD2130331A123456
  * B 180: WDD2462421N123456
  * GLA 200: WDC1569431J123456
  * S 500 Cabrio: WDD2174821A123456
  * Smart fortwo turbo: WME4533441K012345
* `perspectives` - _optional_ - One or more perspectives as a comma separated String list e.g. 'EXT000,EXT010,INT1'.  The following perspectives are available:
  * EXT000-EXT350: EXT000 defines the front view, EXT010 defines a rotation of 10 degress and so forth.
  * INT1-INT4: These are the 4 available interior perspectives.
  
The default value is EXT020,INT1 if no value is provided.
* `roofOpen` - _optional_ - Set 'true', if you are looking for images with the roof open. This option is only valid for cabrios. Default is 'false'.
* `night` - _optional_ - Set 'true', if you are looking for images with a darker background and the vehicle's headlights turned on. Default is 'false'.

### x_swagger_router_controller__finorvin__vehicle

## License

**flow**ground :- Telekom iPaaS / mercedes-benz-com-image-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
