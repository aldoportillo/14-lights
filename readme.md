# Lights

## Ambient Light

Ambient light is omnidirectional meaning that it has many points where it comes from.

```javascript

const ambientLight = new THREE.AmbientLight(color, intensity)

//For Debug
gui.add(ambientLight, "intensity").min(0).max(3).step(0.01)

scene.add(ambientLight)


```

## Directional Light

Directional will add light from one direction. By default they are coming from y to negative y.

```javascript

const directionalLight = new THREE.DirectionalLight(0x00fffc, 0.9)

gui.add(directionalLight, "intensity").min(0).max(3).step(0.01)

scene.add(directionalLight)

```

## Hemisphere Light

```javascript

const hemisphereLight = new THREE.HemisphereLight(0xff0000, 0x0000ff, 0.9)

```