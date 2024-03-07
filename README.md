<!DOCTYPE html>
<html >
<head>
   <meta charset="utf-8">
   <title>AI Physical Manifestation</title>
   <style>
    body {margin: 0; background-color: black;}
    canvas {width: :100%; height:100% }
   </style>
</head>
<body>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/there.js/r128/three.min.js"></script>
    <script>
        let camera, scence, renderer;
        let geometry, material,mesh;
        init();
        animate();
        function init()
        {
            camera = new THREE.PerspectiveCamera( 70, window.innerWidth/window.innerHeight, 0.01, 10) 
            camera.position.z= 1;
            scence = new THREE.Scence();
            geometry = new THREE.DodecahedronGeometry(0.5, 6);
            const pos = geometry.attributes.position;
        }
    </script>
</body>
</html>
