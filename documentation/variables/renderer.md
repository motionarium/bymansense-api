# 🎨 Renderer

## Types:

### Vector

`Vector(x, y, z)`

### Color

`Color.new(r, g, b, a)`

## Functions:

### renderer.world\_to\_screen

`renderer.world_to_screen(position: vector)`

| Name     | Type     | Description                                   |
| -------- | -------- | --------------------------------------------- |
| position | `vector` | [Position in world space](renderer.md#vector) |

### renderer.create\_font

`renderer.create_font(name: string, size: number, size: number, flags: boolean)`

| Name  | Type      | Description                   |
| ----- | --------- | ----------------------------- |
| name  | `string`  | Font that will be initialized |
| size  | `number`  | Size of the font              |
| flags | `boolean` | ???                           |

### renderer.draw\_text

{% tabs %}
{% tab title="renderer.draw_text" %}
`renderer.draw_text(font: FontObject, x: vector, y: vector, color: color, text: any)`

| Name  | Type         | Description                            |
| ----- | ------------ | -------------------------------------- |
| font  | `FontObject` | Font object                            |
| x, y  | `vector`     | Screen position                        |
| color | `color`      | [Color of the text](renderer.md#color) |
| text  | `any`        | Text that will be drawn                |
{% endtab %}

{% tab title="renderer.draw_text_centered" %}
`renderer.draw_text_centered(font: FontObject, x: vector, y: vector, color: color, center_x: boolean, center_y: boolean, text: any)`

| Name      | Type         | Description                            |
| --------- | ------------ | -------------------------------------- |
| font      | `FontObject` | Font object                            |
| x, y      | `vector`     | Screen position                        |
| color     | `color`      | [Color of the text](renderer.md#color) |
| center\_x | `boolean`    | Centered text by x                     |
| center\_y | `boolean`    | Centered text by y                     |
| text      | `any`        | Text that will be drawn                |
{% endtab %}
{% endtabs %}

### renderer.draw\_line

`renderer.draw_line(position_a: vector, position_b: vector, color: color)`

| Name        | Type     | Description                            |
| ----------- | -------- | -------------------------------------- |
| position\_a | `vector` | Start position                         |
| position\_b | `vector` | End position                           |
| color       | `color`  | [Color of the line](renderer.md#color) |

### renderer.draw\_rect

{% tabs %}
{% tab title="renderer.draw_rect" %}
`render.draw_rect(position: vector, height: number, width: number, color: color)`

| Name     | Type     | Description                                 |
| -------- | -------- | ------------------------------------------- |
| position | `vector` | Position                                    |
| height   | `number` | Height of the rectangle                     |
| width    | `number` | Width of the rectangle                      |
| color    | `color`  | [Color of the rectangle](renderer.md#color) |
{% endtab %}

{% tab title="renderer.draw_rect_filled" %}
`render.draw_rect_filled(position: vector, height: number, width: number, color: color)`

|          |          |                                             |
| -------- | -------- | ------------------------------------------- |
| position | `vector` | Position                                    |
| height   | `number` | Height of the rectangle                     |
| width    | `number` | Width of the rectangle                      |
| color    | `color`  | [Color of the rectangle](renderer.md#color) |
{% endtab %}

{% tab title="renderer.draw_rect_filled_gradient" %}
`renderer.draw_rect_filled_gradient(position: vector, height: number, width: number, color_first: color, color_second: color, orientation: number`

| Name          | Type     | Description                                                                                                                                             |
| ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| position      | `vector` | Position                                                                                                                                                |
| height        | `number` | Height of the rectangle                                                                                                                                 |
| width         | `number` | Width of the rectangle                                                                                                                                  |
| color\_first  | `color`  | [First color of the rectangle](renderer.md#color)                                                                                                       |
| color\_second | `color`  | [Second color of the rectangle](renderer.md#color)                                                                                                      |
| orientation   | `number` | <p><mark style="color:green;"><code>1</code></mark> is horizantal gradient<br><mark style="color:green;"><code>0</code></mark> is vertical gradient</p> |
{% endtab %}
{% endtabs %}

### renderer.draw\_circle

{% tabs %}
{% tab title="renderer.draw_circle" %}
`renderer.draw_circle(position: vector, dots: number, radius: number, color: color)`

| Name     | Type     | Description                              |
| -------- | -------- | ---------------------------------------- |
| position | `vector` | Position                                 |
| dots     | `number` | Amount of dots in the circle             |
| radius   | `number` | Radius of the circle in pixels           |
| color    | `color`  | [Color of the circle](renderer.md#color) |
{% endtab %}

{% tab title="renderer.draw_circle_filled" %}
`renderer.draw_circle_filled(position: vector, dots: number, radius: number, color: color)`

| Name     | Type     | Description                              |
| -------- | -------- | ---------------------------------------- |
| position | `vector` | Position                                 |
| dots     | `number` | Amount of dots in the circle             |
| radius   | `number` | Radius of the circle in pixels           |
| color    | `color`  | [Color of the circle](renderer.md#color) |
{% endtab %}
{% endtabs %}

### renderer.draw\_triangle

`renderer.draw_triangle(position_a: vector, position_b: vector, position_c: vector, color: color)`

| Name        | Type     | Description                                |
| ----------- | -------- | ------------------------------------------ |
| position\_a | `vector` | First position                             |
| position\_b | `vector` | Second position                            |
| position\_c | `vector` | Third position                             |
| color       | `color`  | [Color of the triangle](renderer.md#color) |

### renderer.draw\_particles

`renderer.draw_particles(vector: vector)`

| Name   | Type     | Description                    |
| ------ | -------- | ------------------------------ |
| vector | `vector` | [Position](renderer.md#vector) |
