Hi there, I'm Antony Toro Zapata 👋
🚀 Software Development Student | Backend & Full-Stack Developer

<p align="center">
<a href="mailto:torozaapata2009@gmail.com">📧 Contact Me</a>
</p>

👨‍💻 Sobre mí

Soy estudiante de Tecnología en Desarrollo de Software en el SENA, en el Centro Textil y de Gestión Industrial. Me apasiona el ciclo de vida del software, la arquitectura de bases de datos relacionales y el desarrollo backend seguro y eficiente.

🎓 Formación: Tecnólogo en Desarrollo de Software (SENA) y Técnico en Desarrollo de Software (Media Técnica).
💼 Experiencia: Aprendiz de Desarrollo de Software en proyectos formativos SENA y desarrollador web freelance.
🛡️ Enfoque en calidad: Consultas preparadas (parameter binding) para prevenir vulnerabilidades y estructuración de requerimientos bajo el estándar ISO/IEC 25010.
🎯 Objetivo: Aplicar mis competencias técnicas en desarrollo backend y full-stack en entornos profesionales.
🛠️ Technical Skills
💻 Lenguajes de programación

<p>
<img src="https://skillicons.dev/icons?i=php,js,html,css" alt="PHP, JavaScript, HTML y CSS" />
</p>

⚙️ Backend & Bases de datos

<p>
<img src="https://skillicons.dev/icons?i=nodejs,express,mysql,postgres" alt="Node.js, Express, MySQL y PostgreSQL" />
</p>

🎨 Frontend & UI/UX

<p>
<img src="https://skillicons.dev/icons?i=react,tailwind,bootstrap" alt="React, Tailwind CSS y Bootstrap" />
</p>

🔧 Herramientas & DevOps

<p>
<img src="https://skillicons.dev/icons?i=git,github,vscode,linux" alt="Git, GitHub, VS Code y Linux" />
</p>

🧠 Habilidades blandas
Habilidad	Descripción
🧩 Resolución de problemas	Análisis y depuración de código, optimización del rendimiento y solución de vulnerabilidades.
👥 Trabajo en equipo	Colaboración mediante Git, revisión de código y trabajo conjunto en proyectos.
🗣️ Comunicación asertiva	Identificación de requerimientos funcionales y no funcionales.
📋 Calidad del software	Documentación de casos de uso y aplicación de criterios de calidad basados en ISO/IEC 25010.
⚡ Aprendizaje continuo	Adaptación a tecnologías backend y frontend según las necesidades del proyecto.
📂 Proyectos destacados
🌟 SkillMatch

Sistema integral para la búsqueda de empleo.

Especificación de requerimientos y diagramas UML.
Backend estructurado y base de datos relacional.
Tecnologías: PHP MySQL UML

🔗 Ver repositorio

📅 App de Gestión de Citas Laborales

Aplicación web para organizar y administrar agendas y citas laborales.

Organización de calendarios y programación de citas.
Interfaz web para facilitar la coordinación de actividades.
Tecnologías: JavaScript React Node.js CSS3

🔗 Ver repositorio

🔐 API REST de Autenticación

Servicio backend para la gestión de usuarios y autenticación.

Validación de datos de entrada.
Consultas preparadas y acceso seguro a la base de datos.
Tecnologías: PHP Node.js PostgreSQL MySQL REST API

🔗 Ver repositorio

💻 Código destacado: PHP & Seguridad
<?php

class UserRepository
{
    private PDO $connection;

    public function __construct(PDO $connection)
    {
        $this->connection = $connection;
    }

    public function getUserByEmail(string $email): ?array
    {
        $sql = "SELECT id, username, email, role
                FROM users
                WHERE email = :email
                LIMIT 1";

        $stmt = $this->connection->prepare($sql);

        $stmt->bindValue(':email', $email, PDO::PARAM_STR);
        $stmt->execute();

        $data = $stmt->fetch(PDO::FETCH_ASSOC);

        return $data ?: null;
    }
}

📫 Contacto
📧 Email: torozaapata2009@gmail.com
💻 GitHub: Mis repositorios

<p align="center">
💡 <i>Always learning, building and improving.</i>
</p>
