<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Developer Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: #0d1117;
            color: #c9d1d9;
            line-height: 1.6;
            padding: 40px 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            animation: fadeIn 0.8s ease-in;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .header {
            border-bottom: 1px solid #30363d;
            padding-bottom: 30px;
            margin-bottom: 40px;
        }

        .name {
            font-size: 2.5em;
            font-weight: 600;
            color: #f0f6fc;
            margin-bottom: 8px;
            letter-spacing: -0.5px;
            animation: slideInLeft 0.6s ease-out;
        }

        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .title {
            font-size: 1.25em;
            color: #8b949e;
            font-weight: 400;
            margin-bottom: 20px;
            animation: slideInLeft 0.6s ease-out 0.1s backwards;
        }

        .specialization {
            display: inline-block;
            padding: 6px 16px;
            background: #1f6feb;
            color: #fff;
            border-radius: 6px;
            font-size: 0.9em;
            font-weight: 500;
            animation: slideInLeft 0.6s ease-out 0.2s backwards;
            transition: transform 0.3s ease;
        }

        .specialization:hover {
            transform: scale(1.05);
        }

        .section {
            margin-bottom: 50px;
            animation: fadeInUp 0.6s ease-out backwards;
        }

        .section:nth-child(2) { animation-delay: 0.3s; }
        .section:nth-child(3) { animation-delay: 0.4s; }
        .section:nth-child(4) { animation-delay: 0.5s; }
        .section:nth-child(5) { animation-delay: 0.6s; }
        .section:nth-child(6) { animation-delay: 0.7s; }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .section-title {
            font-size: 1.5em;
            color: #f0f6fc;
            font-weight: 600;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title::before {
            content: '';
            width: 4px;
            height: 24px;
            background: #1f6feb;
            border-radius: 2px;
            animation: expandHeight 0.4s ease-out;
        }

        @keyframes expandHeight {
            from {
                height: 0;
            }
            to {
                height: 24px;
            }
        }

        .description {
            color: #8b949e;
            font-size: 1.05em;
            margin-bottom: 25px;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .tech-category {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 20px;
            transition: all 0.3s ease;
        }

        .tech-category:hover {
            border-color: #1f6feb;
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(31, 111, 235, 0.2);
        }

        .tech-category h3 {
            color: #f0f6fc;
            font-size: 1em;
            font-weight: 600;
            margin-bottom: 12px;
        }

        .tech-list {
            list-style: none;
        }

        .tech-list li {
            color: #8b949e;
            padding: 4px 0;
            font-size: 0.95em;
            transition: color 0.2s ease, transform 0.2s ease;
        }

        .tech-list li:hover {
            color: #1f6feb;
            transform: translateX(5px);
        }

        .expertise-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
        }

        .expertise-item {
            background: #161b22;
            border: 1px solid #30363d;
            padding: 16px 20px;
            border-radius: 6px;
            color: #c9d1d9;
            font-size: 0.95em;
            transition: all 0.3s ease;
        }

        .expertise-item:hover {
            border-color: #1f6feb;
            transform: translateX(5px);
            background: #1a1f26;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }

        .contact-link {
            display: block;
            text-align: center;
            padding: 12px 24px;
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            color: #c9d1d9;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }

        .contact-link:hover {
            background: #1f6feb;
            border-color: #1f6feb;
            color: #fff;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(31, 111, 235, 0.3);
        }

        @media (max-width: 768px) {
            .name {
                font-size: 2em;
            }
            
            .tech-grid, .expertise-grid, .contact-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <h1 class="name">David Fernández Morilla</h1>
            <p class="title">Full Stack Developer</p>
            <span class="specialization">AI Development Specialist</span>
        </header>

        <section class="section">
            <h2 class="section-title">Sobre Mí</h2>
            <p class="description">
                Desarrollador Full Stack especializado en la integración de Inteligencia Artificial en aplicaciones modernas. Experto en Python y PHP, con dominio de sus principales frameworks. Enfocado en crear soluciones escalables que aprovechan APIs de IA y herramientas de última generación para resolver problemas complejos del mundo real.
            </p>
        </section>

        <section class="section">
            <h2 class="section-title">Stack Tecnológico</h2>
            <div class="tech-grid">
                <div class="tech-category">
                    <h3>Frontend</h3>
                    <ul class="tech-list">
                        <li>React / Next.js</li>
                        <li>Vue.js / Nuxt</li>
                        <li>TypeScript / JavaScript</li>
                        <li>Tailwind CSS</li>
                    </ul>
                </div>
                <div class="tech-category">
                    <h3>Backend - Python</h3>
                    <ul class="tech-list">
                        <li>Django</li>
                        <li>Flask</li>
                        <li>FastAPI</li>
                        <li>Pyramid</li>
                    </ul>
                </div>
                <div class="tech-category">
                    <h3>Backend - PHP</h3>
                    <ul class="tech-list">
                        <li>Laravel</li>
                        <li>Symfony</li>
                        <li>CodeIgniter</li>
                        <li>Slim</li>
                    </ul>
                </div>
                <div class="tech-category">
                    <h3>Infraestructura</h3>
                    <ul class="tech-list">
                        <li>Docker / Kubernetes</li>
                        <li>AWS / Azure / GCP</li>
                        <li>PostgreSQL / MySQL</li>
                        <li>MongoDB / Redis</li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="section">
            <h2 class="section-title">Desarrollo con IA</h2>
            <div class="expertise-grid">
                <div class="expertise-item">Integración de APIs de IA (OpenAI, Anthropic, Google AI)</div>
                <div class="expertise-item">Desarrollo de aplicaciones con LLMs</div>
                <div class="expertise-item">Implementación de RAG Systems</div>
                <div class="expertise-item">Prompt Engineering & Optimization</div>
                <div class="expertise-item">AI Agents & Chatbots</div>
                <div class="expertise-item">Procesamiento de Lenguaje Natural</div>
                <div class="expertise-item">LangChain & LlamaIndex</div>
                <div class="expertise-item">Vector Databases & Embeddings</div>
            </div>
        </section>

        <section class="section">
            <h2 class="section-title">Áreas de Enfoque</h2>
            <p class="description">
                • Desarrollo de aplicaciones inteligentes integrando APIs de IA<br>
                • Creación de chatbots conversacionales y asistentes virtuales<br>
                • Implementación de sistemas de búsqueda semántica<br>
                • Automatización de procesos mediante IA<br>
                • Diseño de interfaces conversacionales y sistemas de recomendación<br>
                • Optimización de prompts y flujos de conversación
            </p>
        </section>

        <section class="section">
            <h2 class="section-title">Contacto</h2>
            <div class="contact-grid">
                <a href="#" class="contact-link">GitHub</a>
                <a href="#" class="contact-link">LinkedIn</a>
                <a href="#" class="contact-link">Email</a>
                <a href="#" class="contact-link">Portfolio</a>
            </div>
        </section>
    </div>
</body>
</html>
