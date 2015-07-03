---
ID_PAGE: 5717
PG_TITLE: HemisphericLight
PG_VERSION: 2.0
---

Hemispheric light represents a simple and easy way to simulate realistic ambient light.

An hemispheric light is defined by a direction to the sky and by 3 colors: one for the diffuse (the sky color), one for the ground (the color when the pixel is not towards the sky) and one for the specular.

A tutorial about lights can be found [here](https://github.com/BabylonJS/Babylon.js/wiki/06-Lights)
##new [HemisphericLight](page.php?p=5717)(name, direction, scene)


Creates a new [HemisphericLight](page.php?p=5717) object


####Parameters
 | Name | Type | Description
---|---|---|---
 | name | string | The namme of the light
 | direction | [Vector3](page.php?p=5808) | The direction of the light
 | scene | [Scene](page.php?p=5725) | The scene to create the light into
---

##Extends
##Members

###direction : [Vector3](page.php?p=5808)



The direction of the light


###groundColor : [Color3](page.php?p=5805)



The ground color







##Methods

###setDirectionToTarget(target) &rarr; [Vector3](page.php?p=5808)
Sets the direction of the light using the given target



####Parameters
 | Name | Type | Description
---|---|---|---
 | target | [Vector3](page.php?p=5808) | The given target to lighten
---

###getShadowGenerator() &rarr; [ShadowGenerator](page.php?p=5779)
Returns null




###transferToEffect(effect, directionUniformName, groundColorUniformName) &rarr; void

####Parameters
 | Name | Type | Description
---|---|---|---
 | effect | [Effect](page.php?p=5782) | The given effect
 | directionUniformName | string | The direction uniform name
 | groundColorUniformName | string | The groundColor uniform name
---