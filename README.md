# LiDAR app

Potree LiDAR viewer customization and extension

## Installation

1.	Clone this

    `cd /var/www/vhosts/sitj/htdocs/geo3d`
    
    `git clone git@github.com:SIT-Jura/lidar_app.git`
    
2.	Download last release: https://github.com/potree/potree/releases/tag/1.8
3.	`mkdir potree`
4.	copy-paste `libs` and `build` from the downloaded zip to the `/potree` folder
5.  copy-paste `lidar_app\index.html` to `/var/www/vhosts/sitj/htdocs/geo3d`
6.  Add in `/var/www/vhosts/sitj/conf/proxies.conf`
    
    `ProxyPass "/geo3d" !`
    
En cas de mise à jour du fichier index.html, le copier dans lidar_app avant de faire un git push

## Liste des fichiers

- `index.html` : potree + coordonnées xyz

- `index_simple_sans_xyz.html` : potree uniquement

- `index_xyz.html` : potree + coordonnées xyz, adapation de `index_simple_sans_xyz.html` et de `index_xyz_ne.html`

- `index_xyz_ne.html` : potree + coordonnées xyz, exemple NE

## Utilisation avec paramètres

url `index.html?x=2590502.0&y=1245573.0&z=446`

Exemple : https://geo-test.jura.ch/lidar/index.html?x=2590502.0&y=1245573.0&z=446
