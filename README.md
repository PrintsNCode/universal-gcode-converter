# Conversor universal de G-code

Herramienta web de **un solo archivo HTML** que "injerta" la geometría de un G-code en el perfil de tu impresora. Sirve para pasar un recorrido hecho con herramientas como FullControl a una impresora concreta, sin reescribir a mano el inicio, la purga y el final.

Todo se procesa en tu navegador. El G-code no se sube a ningún sitio.

## Cómo funciona

El conversor reutiliza solo el **recorrido** del G-code de origen y lo coloca dentro de una **plantilla** de tu impresora:

1. **Plantilla del destino**: un G-code que *ya imprime bien* en tu impresora. De ahí se toma el inicio, la purga, el final y el perfil (vale cualquier marca; hay soporte pensado para Anycubic, Snapmaker, Klipper y similares).
2. **G-code a convertir**: el `.gcode` de origen del que quieres aprovechar el recorrido.
3. **Parámetros**: material, temperaturas, ventilador, altura de capa, tamaño de cama, centrado y nombre del objeto. Hay un modo avanzado con textura ondulada (modo jarrón).

El resultado se descarga como un `.gcode` listo para laminar o imprimir.

## Cómo usarlo

1. Descarga **`converter-gcode.html`** (botón *Download raw file* en GitHub, o clona el repo).
2. Ábrelo en tu navegador con doble clic.
3. Arrastra tu plantilla y el G-code de origen. Si quieres probar primero, pulsa **Cargar ejemplo**.
4. Ajusta los parámetros y pulsa convertir.
5. Revisa el registro y descarga el resultado.

## Consejos

- **Prueba siempre el G-code convertido en el visor o en una impresión corta** antes de lanzar una pieza larga. Cada impresora tiene sus particularidades.
- La plantilla manda: cuanto mejor sea tu G-code de referencia, mejor saldrá el resultado.
- Comprueba que el tamaño de cama y la altura de capa coinciden con tu impresora.

## Extras

- Idiomas: ES, EN, FR, DE, PT e IT.
- Tema claro y oscuro.

## Aviso

Se comparte tal cual, sin garantías. Revisa siempre el G-code antes de imprimir. Si te sirve, deja una ⭐.

Hecho por [PrintsNCode](https://github.com/PrintsNCode).
