<!DOCTYPE html>
<html>
  <head>
    <base href="/" />
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Test</title>
    <style>
      body {
        margin: 0;
        padding: 0;
        background: #121212;
        color: #fff;
        font-family: 'Inter', system-ui, -apple-system, sans-serif;
        display: flex;
        height: 100vh;
        overflow: hidden;
      }

      .left-panel {
        width: 280px;
        background: #1a1a1a;
        color: #fff;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        padding: 20px;
        border-right: 2px solid #333;
        box-shadow: 2px 0 8px rgba(0, 0, 0, 0.2);
      }

      .left-panel .title {
        font-size: 24px;
        font-weight: bold;
        margin-bottom: 20px;
        background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
        -webkit-background-clip: text;
        background-clip: text;
        -webkit-text-fill-color: transparent;
        text-align: center;
      }

      .panel-item {
        width: 90%;
        display: flex;
        align-items: center;
        padding: 12px;
        margin: 10px 0;
        background: #333;
        border-radius: 12px;
        cursor: pointer;
        transition: transform 0.3s, background 0.3s;
        text-decoration: none;
        color: white;
      }

      .panel-item:hover {
        background: linear-gradient(135deg, #4ecdc4, #388e8e);
        transform: translateY(-5px);
      }

      .panel-item .icon {
        width: 40px;
        height: 40px;
        margin-right: 15px;
        background: linear-gradient(135deg, #ff6b6b, #4ecdc4);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 18px;
        font-weight: bold;
        color: white;
      }

      .panel-item .text {
        font-size: 16px;
        font-weight: bold;
      }

      .container {
        flex: 1;
        padding: 20px;
        display: flex;
        flex-direction: column;
      }
      .header {
  display: flex;
  justify-content: flex-start; /* Başlık sola hizalanır */
  align-items: center;
  padding: 10px 0;
  border-bottom: 2px solid #333;
}


      .title {
        font-size: 28px;
        font-weight: bold;
        background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
        -webkit-background-clip: text;
        background-clip: text;
        -webkit-text-fill-color: transparent;
      }

      #editor {
        width: 100%;
        height: 50vh;
        margin: 20px 0;
        border-radius: 8px;
        overflow: hidden;
        border: 2px solid #333;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        animation: fadeIn 1s ease-in-out;
      }

      #output {
        width: 100%;
        height: 20vh;
        margin: 20px 0;
        padding: 10px;
        border-radius: 8px;
        background: #1e1e1e;
        color: #00ff00;
        font-family: monospace;
        font-size: 14px;
        overflow-y: auto;
        border: 2px solid #333;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        animation: fadeIn 1s ease-in-out;
      }

      .execute-btn {
  background: linear-gradient(135deg, #4ecdc4, #1a535c);
  color: #fff;
  border: none;
  padding: 12px 24px;
  font-size: 16px;
  font-weight: bold;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
  position: absolute; /* Konumlandırmayı mutlak yapıyoruz */
  right: 20px; /* Sağda sabit duracak */
  top: 10px; /* Üstten sabitleme */
}


.execute-btn:hover {
  background: linear-gradient(135deg, #4ecdc4, #388e8e);
  transform: translateY(-2px);
}

.execute-btn:active {
  transform: translateY(0);
  background: #45b7b0;
}

      @keyframes fadeIn {
        from {
          opacity: 0;
          transform: translateY(-10px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }
    </style>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.36.1/min/vs/loader.min.js"></script>
  </head>
  <body>
    <div class="left-panel">
      <div class="title">Navigation</div>
      <div class="panel-item" onclick="alert('Executer selected')">
        <div class="icon">E</div>
        <div class="text">Executer</div>
      </div>
      <div class="panel-item" onclick="alert('ScriptHub selected')">
        <div class="icon">S</div>
        <div class="text">ScriptHub</div>
      </div>
      <div class="panel-item" onclick="alert('Discord selected')">
        <div class="icon">D</div>
        <div class="text">Discord</div>
      </div>
    </div>
    <div class="container">
      <div class="header">
        <div class="title">Test Executor</div>
        <button class="execute-btn" onclick="executeScript()">Execute</button>
      </div>
      <div id="editor"></div>
      <div id="output">Output will appear here...</div>
    </div>
    <script>
      require.config({
        paths: {
          vs: 'https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.36.1/min/vs'
        }
      });

      window.MonacoEnvironment = {
        getWorkerUrl: function() {
          return `data:text/javascript;charset=utf-8,${encodeURIComponent(`
self.MonacoEnvironment = {
  baseUrl: 'https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.36.1/min/'
};
importScripts('https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.36.1/min/vs/base/worker/workerMain.js');`)};`
        }
      };

      require(['vs/editor/editor.main'], function() {
        let editor = monaco.editor.create(document.getElementById('editor'), {
          value: 'print("This is a test UI. Replace it with your own logic.")',
          language: 'lua',
          theme: 'vs-dark',
          automaticLayout: true,
          minimap: {
            enabled: false
          },
          fontSize: 14,
        });

        window.executeScript = function() {
          const editorContent = editor.getValue();
          const outputDiv = document.getElementById('output');

          console.log("Editor content:", editorContent);

          try {
            fetch('http://localhost:5000/message', {
              method: 'POST',
              headers: { 'Content-Type': 'application/json' },
              body: JSON.stringify({ content: editorContent })
            })
            .then(response => response.json())
            .then(data => {
              console.log("Server responded:", data);
              outputDiv.innerText = data.result || "Execution completed successfully!";
            })
            .catch(error => {
              console.error("Error:", error);
              outputDiv.innerText = "An error occurred during execution.";
            });
          } catch (e) {
            console.error("Error while sending JSON:", e);
            alert("There was an issue sending the JSON data.");
            outputDiv.innerText = "Error: Could not send data.";
          }
        };
      });
    </script>
  </body>
</html>
