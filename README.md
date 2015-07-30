# pysafet_curso
Archivos para configuración e instalación, y ejemplos de PySafet

----------------------------------
### Conectarse a la base de datos
Para conectarse con la base de datos es necesario editar el archivo de configuración del .safet 
auth.conf en donde se le colocará psql si se desea conectar con postgres, a su vez se le añade 
el nombre de la base de datos, el usuario y la contraseña.
NOTA: si ocurre un error es posible que sea por la configuracion del postgres, se le debe colocar
trust en vez de md5 en el archivo de configuración de postgres.

### FlowFiles
flowfiles es una carpeta en donde se almacenan los xml para la generación de los graficos.
aqui se deberá consultar el campo de la tabla a calcular el porcentaje y cantidad de cada estatus.
Ej. se desea cnsultar cuantos registros estan en espera, solo se consulta el estatus de la tabla correspondiente que diga 
que el estatus sea igual al consultado.
