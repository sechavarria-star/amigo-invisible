# Amigo Invisible · HP

Web app estática (un solo archivo, sin backend) para organizar el sorteo de amigo invisible
con identidad de marca HP.

## Cómo funciona
- El organizador define reglas (presupuesto, temática, fecha, lugar), agrega participantes y
  exclusiones (parejas que no se tocan), y hace el sorteo.
- El sorteo se calcula **en el navegador** (derangement con restricciones).
- Cada participante recibe un **link secreto único** con su asignación cifrada (XOR + base64)
  dentro de la URL. Solo quien abre el link ve a quién regala — ni el organizador lo ve.
- Reparto por **WhatsApp** o copiando el link.

## Stack
HTML/CSS/JS puro. Sin servidor, sin cuentas, sin emails. Se publica en GitHub Pages.

## Desarrollo
Abrir `index.html` en el navegador, o servir la carpeta:

```bash
python3 -m http.server 4178
```
