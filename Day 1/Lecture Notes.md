# Summary Python for Data Analysts
### Day 1
------------------------------

## Virtual Environment Preparation

- Environment adalah lingkungan ketika kita bekerja menggunakan python. Environment sendiri terdiri dari python interpreter dan beberapa package/library. 
- Kernel adalah penghubung/konektor antara environment dan third-party (Jupyter notebook, Jupyter Lab, dll)
- Package adalah pustaka/library yang dibutuhkan untuk melakukan task tertentu selama kita bekerja dengan python
- Cek apakah Anaconda sudah terinstal dengan perintah 
  ```
  conda --version
  ```
- Jika perintah conda tidak dikenali, tambahkan direktori Anaconda ke PATH atau gunakan Anaconda Prompt
- Membuat environment baru menggunakan perintah 
  ```
  conda create --name <ENV_NAME> python=<PYTHON_VER>

  atau 

  conda create -n <ENV_NAME> python=<PYTHON_VER>

  ```
- Melihat environment yang telah dibuat menggunakan perintah 

  ```
  conda env list
  ``` 
  untuk melihat semua daftar environmentnya. Tanda asterik(*), menandakan environment yang sedang aktif di gunakan

- Untuk mengubah ke aktif environment dapat menggunakan 
  ```
  conda activate <ENV_NAME>
  ``` 
- Untuk install kernel pada environment yang baru, kita butuh untuk menginsal ipykernel package. Gunakan perintah 
    ```
    conda install -c anaconda  ipykernel
    ``` 
    pada environment yang baru dibuat

- Untuk mengkonfirmasi dan mendaftarkan kernel di environment baru gunakan perintah:

  
    ```
    python -m ipykernel install --user --name <KERNEL_NAME> 
    ```
    untuk enable kernel pada environment tersebut

- Untuk menonaktifkan virtual environment bisa menggunakan perintah : 
    ```
    conda deactivate
    ```

## Jupyter Notebook Shortcuts
Anda dapat menggunakan ctrl + shift + p untuk melihat semua shortcut yang dapat digunakan.

Ada 2 mode di jupyter notebook: command mode dan edit mode. Pada command mode Anda dapat melakukan:

- b untuk membuat cell baru
- dd untuk menghapus cell
- c untuk mengcopy cell dan v untuk paste cell
- y mengubah cell ke code cell
- m mengubah cell ke markdown cell
- enter untuk mengaktifkan edit mode

Pada edit mode Anda dapat melakukan:

- ctrl + enter untuk run cell
- ctrl + / untuk menambahkan command pada code cell
- esc untuk mengaktifkan command mode

--------------------------------------------------------
