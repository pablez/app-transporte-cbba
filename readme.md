Prompt: Plan de Proyecto de Aplicación de Transporte Público
1. Stack tecnológico propuesto
Framework de desarrollo: React Native con Expo Go.

Autenticación y base de datos: Firebase (Authentication y Firestore).

Mapas y geolocalización: react-native-maps y la API de OpenRouteService.

API Key de OpenRouteService: eyJvcmciOiI1YjNjZTM1OTc4NTExMTAwMDFjZjYyNDgiLCJpZCI6IjliYzhiZDJmY2RjMTQxNzRhZGRkM2UyZDUyNWRhYmJiIiwiaCI6Im11cm11cjY0In0=

Métodos de pago: Lógica para pagos en efectivo y escáner de códigos QR (con una librería como expo-barcode-scanner).

2. Resumen del proyecto
El objetivo es crear una aplicación móvil de transporte público para Cochabamba, Bolivia, que simule el funcionamiento de plataformas como Uber, pero enfocada en el transporte público. La aplicación tendrá tres roles principales:

Administrador (Admin): Gestiona usuarios, rutas, precios y vehículos.

Conductor: Se registra con su vehículo y puede aceptar viajes. Su ubicación se muestra en el mapa en tiempo real.

Pasajero: Solicita un servicio, ve la ubicación de los conductores cercanos y realiza el pago.

La aplicación permitirá a los usuarios (pasajeros) ver la ubicación de los vehículos de transporte público en tiempo real, solicitar un servicio, y pagar con diferentes métodos.

3. Funcionalidades clave
Login y Registro: Autenticación segura para los tres roles.

Roles y permisos: El tipo de usuario (pasajero, conductor) determinará las pantallas y funcionalidades a las que tiene acceso.

Gestión de usuarios: La base de datos de Firebase almacenará la información de los usuarios y sus roles.

Geolocalización en tiempo real: Los conductores compartirán su ubicación en tiempo real, la cual será visible para los pasajeros en el mapa.

Interfaz de mapas: Los usuarios verán un mapa interactivo con la ubicación de los vehículos disponibles, utilizando la API de OpenRouteService para la geolocalización y el cálculo de rutas.

Tipos de pasajeros y tarifas: La aplicación manejará 6 tipos de pasajeros, cada uno con un precio de pasaje diferente. La aplicación calculará la tarifa según el tipo de pasajero seleccionado.

General: 2.5 Bs.

Adulto mayor: 1.5 Bs.

Discapacitado: 1.5 Bs.

Universitario: 1 Bs.

Escolar (nivel primaria): 0.5 Bs.

Escolar (nivel secundaria): 1 Bs.

Métodos de pago: Se implementará el pago en efectivo y mediante escaneo de código QR.

4. Entregables
Estructura de la aplicación: Pantallas de login, registro, conductor, pasajero y administrador.

Lógica de autenticación: Funcionalidad para login y registro con Firebase.

Funcionalidad de mapas: Visualización y seguimiento de la ubicación en tiempo real.

Implementación de roles: Reglas de negocio para diferenciar los 3 roles de usuario.

Lógica de precios: Cálculo de tarifas según el tipo de pasajero.

Funcionalidad de pagos: Lógica para pagos en efectivo y el escáner de QR.