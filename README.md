
# Asturias Rural accessibility

Estudio rápido de accesibilidad rural en Asturias.

## Instalación

Usamos python sobre anaconda para poder replicar más facilmente los resultados:

* [Instalar anaconda](https://conda.io/docs/installation.html)
* Clonar este repositorio git.
* Recrear el entorno anaconda con el fichero `environment.yml` de este repositorio.
    ```sh
    conda env create -f environment.yml
    ```
* Activar el nuevo entrono "asturias".
    ```sh
    source activate asturias
    ```
* arrancar `jupyter`. Se abrirá la dirección [http://localhost:8888](http://localhost:8888)
```sh
jupyter notebook
```

**Posibles problemas**
En caso de error al importar módulos que deberían existis, hay que asegurarse que los ejecutables que se están usando son los correspondientes del entorno activo de conda. Para comprobarlo, se puede correr `which ipyhon | grep asturias` o `which jupyter | grep asturias`, `ipython -c "import sys;print(sys.modules)" | grep asturias`, o  `python -c "import sys;print(sys.modules)" | grep asturias`. En caso de dar error posiblemente hay que reinstalar `jupyter`, o borrar los kernel de jupyter (`jupyter kernelspec list`)
