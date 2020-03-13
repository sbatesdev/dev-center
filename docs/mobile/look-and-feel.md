---
id: look-feel
title: Customize the Look and Feel
---

Geocortex Mobile's appearance is built around two concepts: Theme and Layout.

The theme controls the color scheme of the app. TODO @felicity - is there a theme switcher now? The color scheme for different themes is defined in branding component of the the [app.config json](concepts-app-config).

### Theming with the Branding Component

This example shows two pre-defined themes that are included with Mobile, light and dark. Custom themes can be added to Mobile's included themes, and selected by changing `activeTheme` property of the branding component.
The branding component can be found and edited in the [`app.json`](quick-start#editing-the-layout-and-config).

:::note
Color properties can be excluded from a theme; The application will choose a default color instead.
:::

```json
    {
      "$type": "branding",
      "id": "branding",
      "activeTheme": "light",
      "themes": [
        {
          "id": "dark",
          "colors": {
            "emphasizedButtonBackground": [ 26, 114, 196, 255 ],
            "emphasizedButtonBackgroundDisabled": [ 137, 184, 228, 255 ],
            "emphasizedButtonBackgroundHover": [ 227, 239, 249, 255 ],
            "emphasizedButtonBorder": [ 181, 211, 238, 255 ],
            "emphasizedButtonBorderDisabled": [ 19, 85, 147, 255 ],
            "emphasizedButtonBorderHover": [ 26, 114, 196, 255 ],
            "emphasizedButtonForeground": [ 255, 255, 255, 255 ],
            "emphasizedButtonForegroundDisabled": [ 19, 85, 147, 255 ],
            "emphasizedButtonForegroundHover": [ 23, 100, 171, 255 ],
            "emphasizedButtonIcon": [ 255, 255, 255, 255 ],
            "emphasizedButtonIconDisabled": [ 19, 85, 147, 255 ],
            "emphasizedButtonIconHover": [ 26, 114, 196, 255 ],
            "buttonBackground": [ 64, 64, 68, 255 ],
            "buttonBackgroundDisabled": [ 114, 114, 121, 255 ],
            "buttonBackgroundHover": [ 255, 255, 255, 255 ],
            "buttonBorder": [ 196, 196, 201, 255 ],
            "buttonBorderDisabled": [ 173, 173, 180, 255 ],
            "buttonBorderHover": [ 26, 114, 196, 255 ],
            "buttonForeground": [ 255, 255, 255, 255 ],
            "buttonForegroundDisabled": [ 196, 196, 201, 255 ],
            "buttonForegroundHover": [ 26, 114, 196, 255 ],
            "buttonIcon": [ 255, 255, 255, 255 ],
            "buttonIconDisabled": [ 196, 196, 201, 255 ],
            "buttonIconHover": [ 26, 114, 196, 255 ],
            "inputBorder": [ 196, 196, 201, 255 ],
            "primaryAccent": [ 227, 239, 249, 255 ],
            "primaryAccentDisabled": [ 130, 130, 138, 255 ],
            "primaryAccentHover": [ 196, 196, 201, 255 ],
            "primaryAccentLarge": [ 137, 184, 228, 255 ],
            "primaryBackground": [ 81, 81, 86, 255 ],
            "primaryBorder": [ 114, 114, 121, 255 ],
            "primaryForeground": [ 255, 255, 255, 255 ],
            "primaryForegroundDisabled": [ 130, 130, 138, 255 ],
            "secondaryBackground": [ 64, 64, 68, 255 ],
            "secondaryBorder": [ 97, 97, 103, 255 ],
            "secondaryForeground": [ 196, 196, 201, 255 ],
            "tabPrimaryForeground": [ 196, 196, 201, 255 ],
            "tabSecondaryForeground": [ 255, 255, 255, 255 ],
            "inlineTableHeaderBackground": [ 64, 64, 68, 255 ],
            "inlineTableRowBackground": [ 97, 97, 103, 255 ],
            "inlineTableBorder": [ 130, 130, 138, 255 ],
            "accentIconBackground": [ 255, 255, 255, 255 ],
            "accentIconForeground": [ 26, 114, 196, 255 ],
            "accentIconBackgroundHover": [ 255, 255, 255, 255 ],
            "accentIconBorder": [ 255, 255, 255, 255 ],
            "accentIconBorderHover": [ 255, 255, 255, 255 ],
            "accentIconForegroundHover": [ 26, 114, 196, 255 ],
            "disabledIconFill": [ 130, 130, 138, 255 ],
            "alertAmberBackground": [ 191, 83, 0, 255 ],
            "alertAmberBackgroundHover": [ 255, 255, 255, 255 ],
            "alertAmberBorder": [ 191, 83, 0, 255 ],
            "alertAmberBorderHover": [ 191, 83, 0, 255 ],
            "alertAmberForeground": [ 255, 255, 255, 255 ],
            "alertAmberForegroundHover": [ 191, 83, 0, 255 ],
            "alertAmberIcon": [ 255, 255, 255, 255 ],
            "alertAmberIconHover": [ 191, 83, 0, 255 ],
            "alertBackgroundDisabled": [ 114, 114, 121, 255 ],
            "alertBorderDisabled": [ 114, 114, 121, 255 ],
            "alertForegroundDisabled": [ 196, 196, 201, 255 ],
            "alertIconDisabled": [ 196, 196, 201, 255 ],
            "alertGreenBackground": [ 0, 128, 64, 255 ],
            "alertGreenBackgroundHover": [ 255, 255, 255, 255 ],
            "alertGreenBorder": [ 0, 128, 64, 255 ],
            "alertGreenBorderHover": [ 0, 128, 64, 255 ],
            "alertGreenForeground": [ 255, 255, 255, 255 ],
            "alertGreenForegroundHover": [ 0, 128, 64, 255 ],
            "alertGreenIcon": [ 255, 255, 255, 255 ],
            "alertGreenIconHover": [ 0, 128, 64, 255 ],
            "alertRedBackground": [ 178, 34, 34, 255 ],
            "alertRedBackgroundHover": [ 255, 255, 255, 255 ],
            "alertRedBorder": [ 178, 34, 34, 255 ],
            "alertRedBorderHover": [ 178, 34, 34, 255 ],
            "alertRedForeground": [ 255, 255, 255, 255 ],
            "alertRedForegroundHover": [ 178, 34, 34, 255 ],
            "alertRedIcon": [ 255, 255, 255, 255 ],
            "alertRedIconHover": [ 178, 34, 34, 255 ],
            "itemSelectedBackground": [ 16, 71, 122, 255 ],
            "itemHoverBackground": [ 26, 114, 196, 255 ]
          }
        },
        {
          "id": "light",
          "colors": {
            "emphasizedButtonBackground": [ 26, 114, 196, 255 ],
            "emphasizedButtonBackgroundDisabled": [ 181, 211, 238, 255 ],
            "emphasizedButtonBackgroundHover": [ 227, 239, 249, 255 ],
            "emphasizedButtonBorder": [ 26, 114, 196, 255 ],
            "emphasizedButtonBorderDisabled": [ 181, 211, 238, 255 ],
            "emphasizedButtonBorderHover": [ 26, 114, 196, 255 ],
            "emphasizedButtonForeground": [ 255, 255, 255, 255 ],
            "emphasizedButtonForegroundDisabled": [ 19, 85, 147, 255 ],
            "emphasizedButtonForegroundHover": [ 19, 85, 147, 255 ],
            "emphasizedButtonIcon": [ 255, 255, 255, 255 ],
            "emphasizedButtonIconDisabled": [ 19, 85, 147, 255 ],
            "emphasizedButtonIconHover": [ 26, 114, 196, 255 ],
            "buttonBackground": [ 255, 255, 255, 255 ],
            "buttonBackgroundDisabled": [ 219, 219, 222, 255 ],
            "buttonBackgroundHover": [ 26, 114, 196, 255 ],
            "buttonBorder": [ 114, 114, 121, 255 ],
            "buttonBorderDisabled": [ 173, 173, 180, 255 ],
            "buttonBorderHover": [ 255, 255, 255, 255 ],
            "buttonForeground": [ 26, 114, 196, 255 ],
            "buttonForegroundDisabled": [ 151, 151, 159, 255 ],
            "buttonForegroundHover": [ 255, 255, 255, 255 ],
            "buttonIcon": [ 26, 114, 196, 255 ],
            "buttonIconHover": [ 255, 255, 255, 255 ],
            "buttonIconDisabled": [ 151, 151, 159, 255 ],
            "inputBorder": [ 114, 114, 121, 255 ],
            "primaryAccent": [ 26, 114, 196, 255 ],
            "primaryAccentDisabled": [ 151, 151, 159, 255 ],
            "primaryAccentHover": [ 114, 114, 121, 255 ],
            "primaryAccentLarge": [ 26, 114, 196, 255 ],
            "primaryBackground": [ 255, 255, 255, 255 ],
            "primaryBorder": [ 219, 219, 222, 255 ],
            "primaryForeground": [ 64, 64, 68, 255 ],
            "primaryForegroundDisabled": [ 196, 196, 201, 255 ],
            "secondaryBackground": [ 242, 242, 243, 255 ],
            "secondaryBorder": [ 196, 196, 201, 255 ],
            "secondaryForeground": [ 81, 81, 86, 255 ],
            "tabPrimaryForeground": [ 26, 114, 196, 255 ],
            "tabSecondaryForeground": [ 64, 64, 68, 255 ],
            "inlineTableHeaderBackground": [ 219, 219, 222, 255 ],
            "inlineTableRowBackground": [ 242, 242, 243, 255 ],
            "inlineTableBorder": [ 196, 196, 201, 255 ],
            "accentIconBackground": [ 255, 255, 255, 255 ],
            "accentIconForeground": [ 26, 114, 196, 255 ],
            "accentIconBackgroundHover": [ 255, 255, 255, 255 ],
            "accentIconBorder": [ 114, 114, 121, 255 ],
            "accentIconBorderHover": [ 114, 114, 121, 255 ],
            "accentIconForegroundHover": [ 26, 114, 196, 255 ],
            "disabledIconFill": [ 130, 130, 138, 255 ],
            "alertAmberBackground": [ 191, 83, 0, 255 ],
            "alertAmberBackgroundHover": [ 255, 255, 255, 255 ],
            "alertAmberBorder": [ 191, 83, 0, 255 ],
            "alertAmberBorderHover": [ 191, 83, 0, 255 ],
            "alertAmberForeground": [ 255, 255, 255, 255 ],
            "alertAmberForegroundHover": [ 191, 83, 0, 255 ],
            "alertAmberIcon": [ 255, 255, 255, 255 ],
            "alertAmberIconHover": [ 191, 83, 0, 255 ],
            "alertBackgroundDisabled": [ 219, 219, 222, 255 ],
            "alertBorderDisabled": [ 219, 219, 222, 255 ],
            "alertForegroundDisabled": [ 151, 151, 159, 255 ],
            "alertIconDisabled": [ 151, 151, 159, 255 ],
            "alertGreenBackground": [ 0, 128, 64, 255 ],
            "alertGreenBackgroundHover": [ 255, 255, 255, 255 ],
            "alertGreenBorder": [ 0, 128, 64, 255 ],
            "alertGreenBorderHover": [ 0, 128, 64, 255 ],
            "alertGreenForeground": [ 255, 255, 255, 255 ],
            "alertGreenForegroundHover": [ 0, 128, 64, 255 ],
            "alertGreenIcon": [ 255, 255, 255, 255 ],
            "alertGreenIconHover": [ 0, 128, 64, 255 ],
            "alertRedBackground": [ 178, 34, 34, 255 ],
            "alertRedBackgroundHover": [ 255, 255, 255, 255 ],
            "alertRedBorder": [ 178, 34, 34, 255 ],
            "alertRedBorderHover": [ 178, 34, 34, 255 ],
            "alertRedForeground": [ 255, 255, 255, 255 ],
            "alertRedForegroundHover": [ 178, 34, 34, 255 ],
            "alertRedIcon": [ 255, 255, 255, 255 ],
            "alertRedIconHover": [ 178, 34, 34, 255 ],
            "itemSelectedBackground": [ 227, 239, 249, 255 ],
            "itemHoverBackground": [ 137, 184, 228, 255 ]
          }
        }
      ]
    },
```

### Changing the Visual Layout of an Application

How elements are laid out in a Mobile Application is defined by an apps Layout. [This article](concepts-layout) will teach you how to configure an App's layout and how to leverage it to customize the appearance of Mobile. Further styling within the layout can be done using [Layout Presentation Attributes](http://localhost:3000concepts-advanced-layout#presentation).

TODO - swapping out icons? @Kenny best practices? 
  Wait on GXM consuming the Geocortex Icons package

TODO - specific example with the quickstart?