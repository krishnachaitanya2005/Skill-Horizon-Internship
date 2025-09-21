## Step 1 – Installation & Setup

```
sudo apt update
sudo apt install dvwa -y
sudo dvwa-start
sudo systemctl start apache2
sudo systemctl enable apache2
```
Open DVWA  at `http://127.0.0.1:42001/`.
Click *Create / Reset Database* on `setup.php`, then log in with `admin / password`.
