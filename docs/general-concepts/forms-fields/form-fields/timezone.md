---
sidebar_position: 2
title: Timezone Form Field
---


The **timezone** form field type provides a drop down list of time zones. If the field has a value saved, this value is displayed when the page is first loaded. If not, the default value (if any) is selected.

- **type** (mandatory) must be *timezone*.
- **name** (mandatory) is the unique name of the field.
- **label** (mandatory) (translatable) is the descriptive title of the field.
- **description** (optional) (translatable) is text that will be shown as a tooltip when the user moves the mouse over the field.
- **default** (optional) (translatable) is the default time zone. For example, use '-10' for '(UTC -10:00) Hawaii'.

Implemented by: libraries/src/Form/TimezoneField.php

## Example XML parameter definition

```xml
<field
        name="mytimezone" 
        type="timezone" 
        default="-10" 
        label="Select a timezone" 
        description=""
/>
```
