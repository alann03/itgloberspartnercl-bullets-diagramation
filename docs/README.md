# Bullets Diagramation

El componente _Bullets Diagramation_ brinda una serie de viñetas que apuntan a categorías de la tienda.

![Media Placeholder](/assets/img/bullets-diagramation.png)

## Configuración

### Paso 1 - Agregar el componente a las dependencias de su aplicación

Dentro del archivo `manifest.json` de su aplicación, debe agregar la siguiente dependencia: 

```json
"dependencies": {
  ...
  "itgloberspartnercl.bullets-diagramation": "0.x"
  ...
}
```

### Paso 2 - Declarar el bloque principal en su aplicación

Agregue el bloque `list-context.bullets-group` donde requiera utilizarlo dentro de su aplicación. Por ejemplo: 

```json
{
  "list-context.bullets-group": {
    "props": {
      ...
      "bullets": [
        {
          "image": "assets/img/televisor__bullet--group.jpg",
          "titleBullet": "Televisores",
          "link": {
            "url": "/"
          }
        }
      ...
      ]
    }
  }
}
```

| Nombre de la propiedad | Tipo | Descripción | Valor por defecto |
| -- | -- | -- | -- |
| `image` | `String` | Imágen del bullet | "" |
| `titleBullet` | `String` | Título del bullet | "" |
| `link` | `linkEnum` | Url vinculada al bullet | "" |

Valores posibles de `linkEnum`
| Nombre de la propiedad | Tipo | Descripción | Valor por defecto |
| -- | -- | -- | -- |
| `url` | `String` | Url vinculada al bullet | "" |
| `attributeNofollow` | `Boolean` | Guía al motor de búsqueda para que no rastree el enlace de la página indicada por la etiqueta. | false |
| `attributeTitle` | `String` | Título del atributo | "" |
| `newTab` | `Boolean` | Si se establece en `true` abre una nueva pestaña al hacer clic en la imagen. | false |

## Customización

Para aplicar personalizaciones de CSS en este y otros bloques, siga la guía [Uso de identificadores de CSS para la personalización de la tienda](https://developers.vtex.com/docs/guides/vtex-io-documentation-using-css-handles-for-store-customization).


| CSS HANDLES |
| -- |
| `bullet__container` |
| `bullet__item` |
| `bullet__item--title` |
| `bullet__item--image` |
| `bullet__item--link` |


## Colaboradores

- **Alan Agustín Huismann**
