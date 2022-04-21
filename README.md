# Golang
 ### Auto fill struct vscode 
 * Installasi tool __terminal / cmd__<br>
    ```
    go get -u github.com/davidrjenni/reftools/cmd/fillstruct
    ```

 * Konfigurasi vscode<br>
   - Jalankan vscode 
   - Tekan tahan __ctrl + k, s__<br>
   - Di kolom pencarian, paste perintah di bawah dan tekan __enter__<br>
     ``` 
     - Go: Fill struct
     ```
   - Tekan tanda __+__ di sebelah kiri tulisan __Go: Fill struct__ dan buat __keybinding__
   
 * Cara menggunakan 
   - Buat struct 
   - Inisialisasi struct dan waktu di dalam "{ }" tekan 1-2x keybinding yg dibuat tadi<br>
   <br>
https://user-images.githubusercontent.com/40784871/164478417-616ecd92-ca43-40a7-aa98-21024ef8c703.mp4


# Vscode extensions
 ### code runner
 * Installasi extension<br>
   - Jalankan vscode
   - Tekan __ctrl + p__, paste perintah di bawah dan tekan __enter__
    ```
    - ext install formulahendry.code-runner
    ```
 * Konfigurasi vscode<br>
    - Tekan __ctrl + ,__ atau masuk __settings.json__
    - paste perintah di bawah ke __settings.json__ dan tekan __save__<br>
    ```
    "code-runner.executorMap": {
        "go": "cd $dir && go run $fileName",
    },
    "code-runner.saveAllFilesBeforeRun": true,
    "code-runner.terminalRoot": "/",
    "code-runner.runInTerminal": true,
    "code-runner.clearPreviousOutput": true,
    "code-runner.executorMapByGlob": {
        "*test*.go": "cd $dir && /usr/bin/grader-cli test ."
    },
    ```
    - Sesuaikan lokasi grader-cli
        ```
        "*test*.go": "cd $dir && <lokasi-grader-cli> test ."
        ```
    - Linux
        ```
        "code-runner.terminalRoot": "/" 
        ```
    - Windows
        ```
        "code-runner.terminalRoot": "\\" 
        ```
 * Cara menggunakan
    - Buka file __* .go__ yang akan di gunakan
    - Tekan __ctrl + shift + p__ dan masukkan perintah di bawah dan __enter__
        ```
        Run Code
        ```
    - Menjalakan file __* .go__ tanpa pindah direktori


https://user-images.githubusercontent.com/40784871/164478997-f0ba82fe-fd00-4b78-a6fd-bfa1e9e37409.mp4
     
   -  Menjalakan file __test.go__ tanpa pindah direktori
       
https://user-images.githubusercontent.com/40784871/164479045-43324468-dcde-4b52-a802-df6d38835f7a.mp4


     
 ### Inline Parameters Extended for VSCode
 * Installasi extension<br>
   - Jalankan vscode
   - Tekan __ctrl + p__ dan masukkan perintah di bawah dan __enter__
    ```
    ext install formulahendry.code-runner
    ```
 * Konfigurasi vscode<br>
    - Tekan __ctrl + ,__ atau masuk __settings.json__
    - paste perintah di bawah ke __settings.json__ dan tekan __save__<br>
    ```
    "inline-parameters.go.enabled": true,
    "inline-parameters.go.hintBeforeParameter": true,
    "inline-parameters.go.suppressWhenArgumentMatchesName": true,
    "inline-parameters.go.showVariadicNumbers": true,
    "editor.inlayHints.fontFamily": "'Droid Sans Mono', 'monospace', monospace",
    "editor.inlayHints.fontSize": 13,
    ```
    - Reload vscode<br>

- Mode nonaktif<br>
 ![mode-nonaktif-](https://user-images.githubusercontent.com/40784871/164479136-82a3c89d-80e5-4c71-b13a-a68fe564b644.png)

- Mode aktif<br>
 ![mode-aktif](https://user-images.githubusercontent.com/40784871/164479153-2d20bb7d-63d6-4c01-8073-30b305003e91.png)

 
