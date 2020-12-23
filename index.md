
<!DOCTYPE html>
<html>
  <head>
    <script  type="text/javascript" src="https://codesandbox.io/public/sse-hooks/sse-hooks.4ad272e551a76463eb23e233cae6f6d2.js"></script>

    <link
      rel="stylesheet"
      href="https://unpkg.com/leopard@^1/dist/index.min.css"
    />
  </head>
  <body>
    <button id="greenFlag">Green Flag</button>
    <div id="project"></div>

    <script type="module">
      import project from "./index.js";

      project.attach("#project");

      document.querySelector("#greenFlag").addEventListener("click", () => {
        project.greenFlag();
      });

      // Autoplay
      project.greenFlag();
    </script>
    <script crossorigin type="text/javascript" src="https://codesandbox.io/static/js/watermark-button.d47e1de20.js"></script>
  </body>
</html>
