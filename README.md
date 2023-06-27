# Android_Kotlin_Persistence_PreferenceManager
### This is a project made in Android Studio, using kotlin, we are using Persistance to save information, with the class PreferenceManager and other class like utlis , and MainActivity 


![image](https://github.com/juliaigz/Android_Kotlin_Persistence_PreferenceManager/assets/40221707/4893339b-e9c0-403f-b62b-55c5f1ebfd73)


### MainActivity 

En la clase MainActivity, se inicializan los elementos de vista utilizando los ID correspondientes del archivo XML. Luego, se configuran los botones "Guardar" y "Borrar" con sus respectivos listeners para realizar las operaciones de guardado y borrado de las preferencias. Además, se implementa el método showSavedPreferences para mostrar los datos guardados en las preferencias en los TextViews correspondientes. La lógica de validación y manipulación de preferencias se realiza en los métodos savePreferences y deletePreferences.

![image](https://github.com/juliaigz/Android_Kotlin_Persistence_PreferenceManager/assets/40221707/71d4e89a-6742-49f7-9215-f2745bdc734f)


### Class Preference Manager 

La clase PreferenceManager es responsable de guardar y obtener los valores de las preferencias utilizando el objeto SharedPreferences. Se definen constantes para las claves de cada valor guardado (KEY_INT_VALUE, KEY_TEXT_VALUE, KEY_BOOL_VALUE y KEY_FLOAT_VALUE).

Los métodos saveIntValue, saveTextValue, saveBoolValue y saveFloatValue se utilizan para guardar los valores en las preferencias.

Los métodos getIntValue, getTextValue, getBoolValue y getFloatValue se utilizan para obtener los valores guardados en las preferencias.

El método deletePreferences se encarga de eliminar todas las preferencias guardadas.

![image](https://github.com/juliaigz/Android_Kotlin_Persistence_PreferenceManager/assets/40221707/2478e7f2-6426-4fcc-8d8a-e6c459ca1374)



### Class Utils 

La clase Utils contiene métodos de utilidad para validar los diferentes tipos de valores.

El método isValidInteger verifica si una cadena de texto representa un número entero válido utilizando un bloque try-catch. Si el valor puede convertirse a un entero sin lanzar una excepción, se considera válido y devuelve true, de lo contrario, devuelve false.

El método isValidText utiliza una expresión regular para validar si una cadena de texto contiene solo letras. Utiliza el método matches para comprobar si la cadena cumple con el patrón establecido por la expresión regular. Devuelve true si la cadena contiene solo letras, de lo contrario, devuelve false.

El método isValidFloat verifica si una cadena de texto representa un número decimal válido utilizando un bloque try-catch. Si el valor puede convertirse a un flotante sin lanzar una excepción, se considera válido y devuelve true, de lo contrario, devuelve false.

![image](https://github.com/juliaigz/Android_Kotlin_Persistence_PreferenceManager/assets/40221707/559f541a-06ec-4a93-9c11-6eb9fcfe5642)


### activity_main.xml

El archivo XML incluye los elementos de vista requeridos, como TextView, EditText, RadioGroup y Button. También se han agregado los botones "Borrar" y "Guardar" al final del diseño. 

![image](https://github.com/juliaigz/Android_Kotlin_Persistence_PreferenceManager/assets/40221707/1abfbe4e-068c-4841-bd92-ce2033b8baa0)

