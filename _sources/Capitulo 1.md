---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Capitulo 1

## Mecánica

La mecánica es considerada una ciencia que describe y predice condiciones de reposo o movimiento bajo la acción de diversas cargas, dentro de la ingeniería civil podemos considerar gran cantidad de cargas que a lo largo de la carrera se irán viendo. Esta mecánica que se ha desarrollado a lo largo de la historia, ha sido empleada para resolver problemas de la realidad (ingeniería) , por lo tanto toma en cuenta muchos de los materiales de la realidad, desde aquellos que pueden deformarse hasta los fluidos, como puede apreciar en el siguiente diagrama:

```{figure} 1.svg
---
height: 500px
name: Mechanics and Divisions
---
La Mecánica y sus divisiones
```

Cuando se habla de un elemento rígido, no significa que este nunca experimentará deformaciones , sino más bien las deformaciones son tan pequeñas que no afectarán el equilibrio del sistema. Los elementos rígidos por otro lado si sufren deformaciones sustanciales que son de suma importancia para conseguir el equilibrio, por citar un elemento de este tipo son las columnas esbeltas o de gran altura donde se presentarán momentos de segundo orden (efectos $p-\Delta$ y $\delta$), pero esto no se estudiará en esta primera sección.

## Conceptos fundamentales y Principios

Antes de sumerginos en los principios, es necesario entender los siguientes conceptos:

- Espacio: Lugar donde se encuentra un punto
- Tiempo: Duración de un evento
- Masa: Cantidad de materia
- Fuerza: Representa la acción de un cuerpo sobre otro

La mecánica como hoy la conocemos es producto de los trabajos y estudios realizados por sir Isaac Newton; y aún esta vigente para muchas aplicaciones, siempre en cuando las velocidades de las partículas no superen la velocidad de la luz. Si se supera esta velocidad es necesario recurrir a la teoría de la relatividad propuesta por Einstein. La mecánica clásica como se conoce, ha sido empleada durante siglos en la historia de la humanidad para una inmensa cantidad de proyectos civiles, por ejemplo.

Existen 6 principios fundamentales en la mecánica clásica, estos fueron verificados mediante experimentos o deducciones matemáticas:

```{figure} 2.svg
---
height: 700px
name: Principios de la Mecánica
---
6 Principios Fundamentales de la Mecánica
```

## Sistema de Unidades

Existen 2 sistemas:

- Sistema Internacional (SI)
- Sistema Inglés (Ingles) Americano o Imperial

Es necesario comprender que las cantidades físicas asociadas a estas unidades fueron tomadas de manera arbitraria. A continuación, se definirán 3 unidades básicas y una derivada:


| Unidad Cinética | Unidad | Símbolo |
|------------------|--------|---------|
| Longitud         | Metro  | m       |
| Masa             | Kilogramo | kg    |
| Tiempo           | Segundo | s      |
| Fuerza           | Newton  | N      |

```{note}
Newton (N) = kgf * m/s²
```

Lo mismo en el sistema americano, solo que la unidad derivada es la masa:

| Unidad Cinética | Unidad | Símbolo |
|------------------|--------|---------|
| Longitud         | Pie    | ft      |
| Masa             | Slug   | slug    |
| Tiempo           | Segundo | s      |
| Fuerza           | Libra  | lb      |

```{note}
1/32.2 lbf *s2 / ft = 1 lbm

lbf * s2 / ft = slug
```

```{warning}
lbm $\neq$ lbf
```

## Conversión entre 2 sistemas de unidades

Debemos recordar las siguientes equivalencias:

| Unidad Cinética | Unidad | Símbolo | Equivalencia |
|------------------|--------|---------|--------------|
| Longitud         | Metro  | m       | 1 ft = 0.3048 ft |
| Masa             | Kilogramo | kg    | 1 kg = 2.205 lbm |
| Tiempo           | Segundo | s      | 1 s = 1 s |
| Fuerza           | Newton  | N      | 1 N = 0.225 lbf |

```{note}
g = 32.2 ft/s² = 9.81 m/s²

9.81N = 1kgf ( F=ma $\Rightarrow$ 9.81N = 1kgm*9.81m/s² = 1kgf )
```

```{warning}
1kgf $\neq$ 1kg
```

$$F=ma$$
$$1N=1kg*\frac{m}{s^2}...(1)$$
$$1lbf=1lmb*32.2*\frac{ft}{s^2}...(2)$$

Considerando los siguientes valores, podemos reemplazar en las ecuaciones anteriores:

$$1kg=2.2lbm$$
$$1ft=0.3048m$$

Finalmente, tenemos:

$$1lbf=\frac{1}{2.2}kg*32.2*0.3048*\frac{m}{s^2}=\frac{0.3048*32.2}{2.2}N$$
$$1lbf=4.46N$$
$$1N=0.225lbf$$


## Métodos de resolución de problemas

Dentro de la resolución de problemas es muy importante tener en cuenta los siguientes puntos:

El **diagrama de cuerpo de libre** es uno de ellos, y es de vital importancia ya que a partir de aquí se comienza con la resolución misma del problema. De no realizar un correcto diagrama, todo lo demás será hecho en vano. Para realizar un correcto proceso, se debe considerar el comportamiento de cada elemento del sistema para definir la dirección (sentido y linea de acción) de las fuerzas. El siguiente ejemplo muestra como se comportan los cables cuando un objecto es dispuesto de manera vertical:

```{figure} DCL.svg
---
height: 500px
name: DCL
---
Diagrama de Cuerpo Libre
```

Por otro lado es de mucha importancia considerar la **revisión** de los resultados, antes de brindar una respuesta definitiva. Esto incluye:

- El correcto uso de las *unidades* en los cálculos.
- Revisión de la *coherencia* de los resultados con la realidad.

## Precisión Numérica

Dependiendo de unidad, se considerará hasta 3 o 4 decimales según sea el caso. El hecho de incrementar más decimales será infructuoso.