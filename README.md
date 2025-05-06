# Control de Presupuestos - React + TypeScript + Vite
*📓 [Español](#inicio)*
*📓 [English](#start)*

### <a id="inicio" />
Este proyecto consiste en una aplicación web que al iniciar, aparece un formulario para definir el presupuesto que se tiene de dinero. Al completar el formulario, aparece la interfaz principal, la cual consiste en un modulo que muestra una gráfica circular con el porcentaje del presupuesto gastado y las cantidades de presupuesto disponible y gastado. Se muestra un select para en caso de ser necesario, filtrar por tipo los gastos que se vayan agregando, después del filtro se encuentra la lista de gastos realizados, en caso de no haber agregado ningún gasto, aparecerá el mensaje "No hay gastos". Lo más importante, aparece en la esquina inferior derecha un botón con el signo "+" que al presionar abre una ventana modal en la que se encuentra otro formulario para agregar un gasto nuevo. Se hace uso de localStorage, validación de formularios y modificación de valores en base a ID's.

Algunas de las cosas que se aprendieron con este proyecto son:

### <a  /> useReducer
Se toma un enfoque un tanto diferente a las otras versiones del proyecto ya que se gestiona el estado del carrito en el reducer. Con los reducers se puede agrupar la lógica para que cuando se dispare (dispatch) una acción en alguna parte del proyecto se envien ciertos datos (payload) en caso de necesitarse y sean recibidos tanto dispatch como payload en el reducer y se ejecute código asignado a cada acción.

### <a  /> LocalStorage
Se utilizó localStorage para almacenar los datos de los productos agregados al carrito

### <a  /> Modularidad y Reutilización de Componentes
La reutilización de componentes en este proyecto fue esencialmente necesaria para mostrar los productos y los productos dentro del carrito, evitando código duplicado.

### <a  /> Custom Hooks
Dentro del custom hook, se encuentra la lógica para agregar, eliminar o aumentar la cantidad de elementos agregados al carrito. De igual manera se encuentran varios hooks como useEffect para la parte del localStorage, useMemo para states derivados  y useState para el carrito

### <a  /> Optimización del Rendimiento (Performance)
Además de utilizar componentes, mediante el uso de operadores ternarios, se establece si se renderiza un componente o no, lo que puede mejorar el rendimiento de las aplicaciones web.

### <a  /> Tipado Estricto con TypeScript
Se definieron tipos para los props de los componentes y funciones

### <a  /> Validación de Formularios
Se configuraron los forms de manera que se verifique si el usuario ingresa valores válidos.

### <a  /> Helpers
Se crearon funciones especificas para el formato de fecha y moneda mostrada en la interfaz (formatCurrency y formatDate)

### <a  /> Context
El uso de context en el proyecto sirvió para compartir datos y funciones entre distintos componentes sin necesidad de pasar props "manualmente"

### <a  /> Framework CSS
Se utilizó Bootstrap para manejar los estilos de la página

*📷[Screenshots](#screenshots)*

# Budget Control - React + TypeScript + Vite

### <a id="start" />

This project consists of a web application that, upon launch, displays a form for defining the current budget. Upon completing the form, the main interface appears. It consists of a module showing a pie chart showing the percentage of the budget spent and the amounts of the available and spent budget. A select button is displayed to filter the added expenses by type, if necessary. After the filter, there is a list of expenses incurred. If no expenses have been added, the message "No expenses" appears. Most importantly, a button with a "+" sign appears in the lower right corner. When pressed, it opens a modal window containing another form for adding a new expense. LocalStorage is used, along with form validation and modification of values ​​based on IDs.

Some of the things learned with this project are:

### <a /> useReducer
This takes a slightly different approach than other versions of the project, as the cart state is managed in the reducer. With reducers, you can group logic so that when an action is triggered (dispatch) in some part of the project, certain data (payload) is sent if needed and both dispatch and payload are received in the reducer and code assigned to each action is executed.
### <a  /> LocalStorage
LocalStorage was used to store data for products added to the cart.

### <a  /> Modularity and Components Reusability
Reusing components in this project was essential to display the products and items within the cart, avoiding duplicate code.

### <a  /> Custom Hooks
Inside the custom hook is the logic for adding, removing, or increasing the number of items added to the cart. There are also several hooks, such as useEffect for the localStorage section, useMemo for derived states, and useState for the cart.

### <a  /> Performance Optimization
In addition to using components, by using ternary operators, you can set whether a component is rendered or not, which can improve the performance of web applications.

### <a  /> Strict Typing with TypeScript
Types were defined for component and function props

### <a  /> Form Validation
Forms have been configured to check whether the user enters valid values.

### <a  /> Helpers
Specific functions were created for the date and currency format displayed in the interface (formatCurrency and formatDate)

### <a  /> Context
Using context in this project made it easier to share data and functions between different components without having to pass props "manually"

### <a  /> Framework CSS
Bootstrap was used to handle the page styles

---
### <a id="screenshots" /> 
# Screenshots
![Interfaz](https://github.com/ReploidGI0/control-gastos/blob/main/images/gastos1.PNG "Interfaz")
![Interfaz](https://github.com/ReploidGI0/control-gastos/blob/main/images/gastos2.PNG "Interfaz")
![Interfaz](https://github.com/ReploidGI0/control-gastos/blob/main/images/gastos3.PNG "Interfaz")
![Interfaz](https://github.com/ReploidGI0/control-gastos/blob/main/images/gastos4.PNG "Interfaz")
![Interfaz](https://github.com/ReploidGI0/control-gastos/blob/main/images/gastos5.PNG "Interfaz")

