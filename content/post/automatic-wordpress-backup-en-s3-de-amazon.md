+++
author = "Arturo"
date = 2012-06-13T11:37:22Z
description = ""
draft = false
slug = "automatic-wordpress-backup-en-s3-de-amazon"
title = "Automatic Wordpress Backup en S3 de Amazon"

+++

Una de las tareas a tener en cuenta cuando se mantiene un blog en un hosting propio, es tenerlo respaldado, ojalá en forma diaria y mejor aún en un lugar fuera del propio hospedaje.

<a href="https://wordpress.org/extend/plugins/automatic-wordpress-backup/">Automatic Wordpress Backup</a> hace esta tarea de forma eficiente, genera respaldos automáticos en blog´s bajo la plataforma Wordpress y los sube a la nube de <a href="https://aws.amazon.com/es/s3/">Amazon S3</a>.

El plugins es muy fácil de instalar y de configurar, hay que ingresar el AWS Access Key y la AWS Secret Key de nuestro Bucket en S3, seleccionar si queremos hacer un respaldo de nuestra base de datos junto a las imágenes y si incluímos los archivos también. Y listo, este se ejecutará todos los días o cada vez que queramos, gracias al cron de nuestro Wordpress.

<iframe width="640" height="360" src="http://www.youtube.com/embed/5A-auuJzb4A?rel=0" frameborder="0" allowfullscreen></iframe>

Si quieres mas detalles sobre su instalación, compatibilidad y soporte en general, puedes visitar el <a href="https://www.wordpressbackup.org/">sitio del programa</a>.
