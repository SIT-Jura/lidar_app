# LiDAR app

Potree LiDAR viewer customization and extension

1.	Clone this

    `cd /var/www/vhosts/sitj/htdocs/lidar`
    
    `git clone git@github.com:SIT-Jura/lidar_app.git`
    
2.	Download last release: https://github.com/potree/potree/releases/tag/1.8
3.	`mkdir potree`
4.	copy-paste `libs` and `build` from the downloaded zip to the `/potree` folder
5.  copy-paste `lidar_app\index.html` to `/var/www/vhosts/sitj/htdocs/lidar`
6.  Add in `/var/www/vhosts/sitj/conf/proxies.conf`
    
    `ProxyPass "/lidar" !`
    
En cas de mise à jour du fichier index.html, le copier dans lidar_app avant de faire un git push
