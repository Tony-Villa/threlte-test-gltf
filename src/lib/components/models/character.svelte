<!--
Auto-generated by: https://github.com/threlte/threlte/tree/main/packages/gltf
Command: npx @threlte/gltf@3.0.0-next.6 /Users/tonyvilla/code/apps/portfolio-3d/static/models/character.glb --root /models/ --printwidth 120 --precision 2
-->

<script lang="ts">
	import type { PropTypes } from '$lib/types/types';
  import { T } from '@threlte/core'
  import { useGltf } from '@threlte/extras'

  

  let { fallback, error, children, ref = $bindable(), ...props }: PropTypes = $props()

  const gltf = useGltf('/models/character.glb')
</script>

<T.Group
  bind:ref
  dispose={false}
  {...props}
>
  {#await gltf}
    {@render fallback?.()}
  {:then gltf}
    <T.Group
      position={[2.6, 0.87, -0.09]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    >
      <T.Mesh
        geometry={gltf.nodes.Mesh066.geometry}
        material={gltf.materials.Skin_Asian}
      />
      <T.Mesh
        geometry={gltf.nodes.Mesh066_1.geometry}
        material={gltf.materials.Tom_Hair_Black_Base}
      />
    </T.Group>
    <T.Mesh
      geometry={gltf.nodes.Cap_Front.geometry}
      material={gltf.materials.front_hat}
      position={[2.6, -0.02, -0.09]}
      scale={0.67}
    />
    <T.Group
      position={[2.62, 1.08, -0.01]}
      rotation={[1.65, -0.01, -0.13]}
      scale={0.67}
    >
      <T.Mesh
        geometry={gltf.nodes.Sphere009.geometry}
        material={gltf.materials.corneaMAT}
      />
      <T.Mesh
        geometry={gltf.nodes.Sphere009_1.geometry}
        material={gltf.materials.iris_BrownDarker}
      />
    </T.Group>
    <T.Group
      position={[2.58, 1.08, -0.01]}
      rotation={[1.65, 0.01, 0.13]}
      scale={0.67}
    >
      <T.Mesh
        geometry={gltf.nodes.Sphere008.geometry}
        material={gltf.materials.corneaMAT}
      />
      <T.Mesh
        geometry={gltf.nodes.Sphere008_1.geometry}
        material={gltf.materials.iris_BrownDarker}
      />
    </T.Group>
    <T.Mesh
      geometry={gltf.nodes.EyeBrow.geometry}
      material={gltf.materials.Tom_Hair_Black_Base}
      position={[2.6, 0.87, -0.09]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    />
    <T.Mesh
      geometry={gltf.nodes.Facial_Hair_01.geometry}
      material={gltf.materials.Tom_Hair_Black_Base}
      position={[2.6, 1.03, 0.03]}
      scale={0.51}
    />
    <T.Mesh
      geometry={gltf.nodes.Glasses1_Frame.geometry}
      material={gltf.materials.Glasses_Frame}
      position={[2.6, 0.88, -0.11]}
      rotation={[1.63, 0, 0]}
      scale={0.22}
    />
    <T.Mesh
      geometry={gltf.nodes.Glasses1_Glass.geometry}
      material={gltf.materials.Glasses_Glass}
      position={[2.6, 0.88, -0.11]}
      rotation={[1.63, 0, 0]}
      scale={0.22}
    />
    <T.Mesh
      geometry={gltf.nodes.Hair_Black_Base.geometry}
      material={gltf.materials.Tom_Hair_Black_Base}
      position={[2.6, 0.87, -0.09]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    />
    <T.Group
      position={[2.6, 0.87, -0.09]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    >
      <T.Mesh
        geometry={gltf.nodes.Mesh012.geometry}
        material={gltf.materials.teeth}
      />
      <T.Mesh
        geometry={gltf.nodes.Mesh012_1.geometry}
        material={gltf.materials.gum}
      />
    </T.Group>
    <T.Mesh
      geometry={gltf.nodes.pants.geometry}
      material={gltf.materials.pants}
      position={[2.6, -0.02, -0.05]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    />
    <T.Mesh
      geometry={gltf.nodes.shirtMirror.geometry}
      material={gltf.materials.shirt}
      position={[2.6, -0.02, -0.05]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    />
    <T.Group
      position={[2.6, -0.02, -0.05]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    >
      <T.Mesh
        geometry={gltf.nodes.Mesh003.geometry}
        material={gltf.materials.shoes_01}
      />
      <T.Mesh
        geometry={gltf.nodes.Mesh003_1.geometry}
        material={gltf.materials.shoes_02}
      />
      <T.Mesh
        geometry={gltf.nodes.Mesh003_2.geometry}
        material={gltf.materials.shoes_03}
      />
    </T.Group>
    <T.Mesh
      geometry={gltf.nodes.Tongue.geometry}
      material={gltf.materials.gum}
      position={[2.6, 0.87, -0.09]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    />
    <T.Group
      position={[2.6, 0.87, -0.09]}
      rotation={[Math.PI / 2, 0, 0]}
      scale={0.67}
    >
      <T.Mesh
        geometry={gltf.nodes.Mesh011.geometry}
        material={gltf.materials.teeth}
      />
      <T.Mesh
        geometry={gltf.nodes.Mesh011_1.geometry}
        material={gltf.materials.gum}
      />
    </T.Group>
  {:catch err}
    {@render error?.({ error: err })}
  {/await}

  {@render children?.({ ref })}
</T.Group>
