# Google Cloud Shell

<br>1 . [Getting Started With Cloud Shell](https://cloud.google.com/shell/docs/starting-cloud-shell)
<br>2 . Edit the following index.php with the correct IP address.
```bash
wget https://gist.githubusercontent.com/GedMullen/3cd8591dac1e436e694aa8ab7bdd8d12/raw/a9decaa767693932a3becf3fb1f3203eb5bb12e3/index.php
```
<br>3 . Run a PHP webserver and view the output using Web View. Change the port to 8081. 
```bash
php -S 0.0.0.0:8081
```
<br>4 . [Google Cloud Machine Types](https://cloud.google.com/compute/docs/machine-types). Cloud Shell uses g1-small machine type. MySQL server runs on a n1-standard-1 machine type. 

