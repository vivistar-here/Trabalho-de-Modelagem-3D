<html>
  <head>
    <title>Terceira experiência de RA usando AR.js e A-frame com modelo 3D e marcador hiro</title>
    <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
  </head>
  <body style="margin: 0px; overflow: hidden">
    <a-scene vr-mode-ui="enabled: false" embedded arjs="debugUIEnabled: false">
      <a-assets>
        <a-asset-item id="telefone" src="reieitura animada.glb"></a-asset-item>
      </a-assets>
      <a-marker preset="hiro">
        <a-entity 
	        gltf-model="#telefone">  
          position="0 0 0" 
          rotation="90 0 0" 
          scale="0.5 0.5 0.5"
        </a-entity>
      </a-marker>
      <a-entity camera></a-entity>
    </a-scene>
  </body>
</html>
