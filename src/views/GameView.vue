<!-- <template>
  <div id="unity-container">
      <canvas id="unity-canvas" width=1920 height=1080 tabindex="-1"></canvas>
      <div id="unity-loading-bar">
        <div id="unity-logo"></div>
        <div id="unity-progress-bar-empty">
          <div id="unity-progress-bar-full"></div>
        </div>
      </div>
      <div id="unity-warning"> </div>
    </div>
</template>

<script setup>
import { onMounted } from 'vue'
// export default {
// }
onMounted(() => {
      // window.addEventListener("load", function () {
      //   if ("serviceWorker" in navigator) {
      //     navigator.serviceWorker.register("ServiceWorker.js");
      //   }
      // });

      var container = document.querySelector("#unity-container");
      var canvas = document.querySelector("#unity-canvas");
      var loadingBar = document.querySelector("#unity-loading-bar");
      var progressBarFull = document.querySelector("#unity-progress-bar-full");
      var warningBanner = document.querySelector("#unity-warning");

      // Shows a temporary message banner/ribbon for a few seconds, or
      // a permanent error message on top of the canvas if type=='error'.
      // If type=='warning', a yellow highlight color is used.
      // Modify or remove this function to customize the visually presented
      // way that non-critical warnings and error messages are presented to the
      // user.
      function unityShowBanner(msg, type) {
        function updateBannerVisibility() {
          warningBanner.style.display = warningBanner.children.length ? 'block' : 'none';
        }
        var div = document.createElement('div');
        div.innerHTML = msg;
        warningBanner.appendChild(div);
        if (type == 'error') div.style = 'background: red; padding: 10px;';
        else {
          if (type == 'warning') div.style = 'background: yellow; padding: 10px;';
          setTimeout(function() {
            warningBanner.removeChild(div);
            updateBannerVisibility();
          }, 5000);
        }
        updateBannerVisibility();
      }

      var buildUrl = "Build";
      var loaderUrl = buildUrl + "/WebGL.loader.js";
      var config = {
        dataUrl: buildUrl + "/WebGL.data",
        frameworkUrl: buildUrl + "/WebGL.framework.js",
        codeUrl: buildUrl + "/WebGL.wasm",
        streamingAssetsUrl: "StreamingAssets",
        companyName: "Chora Puma",
        productName: "Awoken",
        productVersion: "1",
        showBanner: unityShowBanner,
      };

      // By default Unity keeps WebGL canvas render target size matched with
      // the DOM size of the canvas element (scaled by window.devicePixelRatio)
      // Set this to false if you want to decouple this synchronization from
      // happening inside the engine, and you would instead like to size up
      // the canvas DOM size and WebGL render target sizes yourself.
      // config.matchWebGLToCanvasSize = false;

      if (/iPhone|iPad|iPod|Android/i.test(navigator.userAgent)) {
        // Mobile device style: fill the whole browser client area with the game canvas:
        var meta = document.createElement('meta');
        meta.name = 'viewport';
        meta.content = 'width=device-width, height=device-height, initial-scale=1.0, user-scalable=no, shrink-to-fit=yes';
        document.getElementsByTagName('head')[0].appendChild(meta);
      }

      loadingBar.style.display = "block";

      var script = document.createElement("script");
      script.src = loaderUrl;
      script.onload = () => {
        createUnityInstance(canvas, config, (progress) => {
          progressBarFull.style.width = 100 * progress + "%";
        }).then((unityInstance) => {
          loadingBar.style.display = "none";
        }).catch((message) => {
          alert(message);
        });
      };
      document.body.appendChild(script);
    });
</script>

<style scoped>

#unity-container { position: fixed; width: 100%; height: 100%; }
#unity-canvas { width: 100%; height: 100%; background: #231F20 }
#unity-loading-bar { position: absolute; left: 50%; top: 50%; transform: translate(-50%, -50%); display: none }
#unity-logo { width: 154px; height: 130px; background: url('unity-logo-dark.png') no-repeat center }
#unity-progress-bar-empty { margin-left: auto; margin-right: auto; width: 141px; height: 18px; margin-top: 10px; background: url('progress-bar-empty-dark.png') no-repeat center }
#unity-progress-bar-full { width: 0%; height: 18px; margin-top: 10px; background: url('progress-bar-full-dark.png') no-repeat center }
#unity-warning { position: absolute; left: 50%; top: 5%; transform: translate(-50%); background: white; padding: 10px; display: none }

</style> -->