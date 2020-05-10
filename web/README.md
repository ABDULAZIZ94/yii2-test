# install php from ondrej private repository
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
sudo apt-get install -y php7.4
# install php dependency
sudo apt install php7.4-mbstring php7.4-xml
# recomended aditional php depencecy
sudo apt install php7.4-bcmath php7.4-bz2 php7.4-curl php7.4-intl php7.4-mbstring php7.4-mysql php7.4-readline php7.4-xml php7.4-zip`
# install composer
sudo apt install composer
# create new yii project
composer create-project — prefer-dist yiisoft/yii2-app-basic basic
# enter project directory and serve it
cd ./basic
php yii serve — port=8888

sudo php yii serve 0.0.0.0 --port=80