# Carlos Garcés Courses Platform

## 🌐 English Version

### Project Summary

This is a backend and frontend platform built with Clean Architecture using .NET 8 for the backend (REST API) and Angular for the frontend. The project is focused on offering online courses in two areas:

* 🌈 Professional House Painting
* 📈 Financial Trading

Carlos Garcés is the creator and instructor for these courses.

### Modules Included

* 🔑 **Authentication** with Azure Active Directory (Azure AD)
* 👤 **User management**
* 📅 **Course catalog** (Trading and Painting)
* 💳 **Payment integration** (Stripe/PayPal)
* 💬 **Testimonials** and feedback
* 📢 **Messaging system** using Azure Service Bus
* 📉 **Admin dashboard** (future feature)

### Backend Stack

* ✅ .NET 8 (latest version)
* ⚖️ Clean Architecture
* 📄 Entity Framework Core (ORM for database access)
* 📆 MySQL (Database)
* ⚡ Azure Service Bus (Messaging system)
* 🌐 Azure App Services (Deployment)
* ✂ Visual Studio Code (Development environment)

### Frontend Stack

* 🔮 Angular
* 📃 HTML/CSS/TypeScript (Migration from current static layout)

### Backend Architecture (Clean)

```
CarlosGarcesApp/
├── Domain/
│   ├── Entities/
│   │   ├── Course.cs
│   │   ├── Testimonio.cs
│   │   └── User.cs
│   └── Interfaces/
│       ├── ICourseRepository.cs
│       └── IUserService.cs
├── Application/
│   ├── DTOs/
│   ├── Services/
│   ├── UseCases/
│   └── Validators/
├── Infrastructure/
│   ├── Data/
│   ├── Services/
│   └── Messaging/
└── WebApi/
    ├── Controllers/
    │   ├── CoursesController.cs
    │   ├── UsersController.cs
    │   └── TestimoniosController.cs
    └── appsettings.json
```

### REST API Usage

| Frontend Feature             | API Endpoint                    | Description                            |
| ---------------------------- | ------------------------------- | -------------------------------------- |
| List Trading Courses         | GET `/api/courses?type=trading` | Load Trading courses from the database |
| List Painting Courses        | GET `/api/courses?type=pintura` | Load Painting courses                  |
| Submit Testimonial           | POST `/api/testimonios`         | Save user testimonial                  |
| Get Testimonials             | GET `/api/testimonios`          | Return testimonials                    |
| Login with Azure AD          | POST `/login`                   | Returns secure token                   |
| Make a Payment               | POST `/api/payment`             | Trigger payment process                |
| Send Contact Form (optional) | POST `/api/contacto`            | Handle form data                       |

---

## 🇪🇸 Versión en Español

### Resumen del Proyecto

Esta es una plataforma con arquitectura limpia desarrollada en .NET 8 para el backend (REST API) y Angular para el frontend. Su enfoque es ofrecer cursos online en dos áreas:

* 🌈 Pintura Profesional para Casas
* 📈 Trading Financiero

Carlos Garcés es el creador e instructor de estos cursos.

### Módulos del Proyecto

* 🔑 **Autenticación** con Azure Active Directory (Azure AD)
* 👤 **Gestión de usuarios**
* 📅 **Catálogo de cursos** (Trading y Pintura)
* 💳 **Pagos integrados** (Stripe/PayPal)
* 💬 **Testimonios y comentarios**
* 📢 **Mensajería interna** con Azure Service Bus
* 📉 **Panel administrativo** (próxima funcionalidad)

### Stack de Backend

* ✅ .NET 8 (versión más reciente)
* ⚖️ Arquitectura limpia (Clean Architecture)
* 📄 Entity Framework Core (ORM para acceso a la BD)
* 📆 MySQL (Base de datos)
* ⚡ Azure Service Bus (Mensajería)
* 🌐 Azure App Services (Despliegue)
* ✂ Visual Studio Code (Entorno de desarrollo)

### Stack de Frontend

* 🔮 Angular
* 📃 HTML/CSS/TypeScript (Migrado desde diseño estático)

### Arquitectura del Backend (Limpia)

```
CarlosGarcesApp/
├── Domain/
│   ├── Entities/
│   │   ├── Course.cs
│   │   ├── Testimonio.cs
│   │   └── User.cs
│   └── Interfaces/
│       ├── ICourseRepository.cs
│       └── IUserService.cs
├── Application/
│   ├── DTOs/
│   ├── Services/
│   ├── UseCases/
│   └── Validators/
├── Infrastructure/
│   ├── Data/
│   ├── Services/
│   └── Messaging/
└── WebApi/
    ├── Controllers/
    │   ├── CoursesController.cs
    │   ├── UsersController.cs
    │   └── TestimoniosController.cs
    └── appsettings.json
```

### Uso de la API REST

| Funcionalidad del Frontend        | Endpoint API                    | Descripción                                    |
| --------------------------------- | ------------------------------- | ---------------------------------------------- |
| Lista de cursos de Trading        | GET `/api/courses?type=trading` | Carga cursos de trading desde la base de datos |
| Lista de cursos de Pintura        | GET `/api/courses?type=pintura` | Carga cursos de pintura                        |
| Enviar testimonio                 | POST `/api/testimonios`         | Guarda testimonio del usuario                  |
| Ver testimonios                   | GET `/api/testimonios`          | Devuelve los comentarios                       |
| Autenticación con Azure AD        | POST `/login`                   | Devuelve token seguro                          |
| Realizar pago                     | POST `/api/payment`             | Inicia proceso de pago                         |
| Formulario de contacto (opcional) | POST `/api/contacto`            | Maneja datos del formulario                    |

---

Ready to start the backend code!
