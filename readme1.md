'use strict';

  function ThreejsScene() {
    this.shapeX = 20;
    this.shapeY = 20;
    this.shapeZ = 20;
    this.shapeColor = 0xF4EBEB;
  }


  ThreejsScene.prototype.init = function () {
    this.scene = new THREE.Scene();
    this.initCamera();
    this.initLight();
    this.initRenderer();
    this.setEventListeners();

    this.initShapes();

    this.render();
  };
