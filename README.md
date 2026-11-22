<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wesia — Seu Estúdio Inteligente de IA</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }

        :root {
            --bg: #050508;
            --bg-alt: #111118;
            --card: #1a1a24;
            --accent: #6366f1;
            --accent-light: #818cf8;
            --text: #f0f0f5;
            --text-muted: #9ca3af;
            --border: #2e2e3f;
        }

        body {
            background: var(--bg);
            color: var(--text);
            line-height: 1.6;
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px;
        }

        header {
            padding: 24px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid var(--border);
        }

        .logo {
            font-size: 28px;
            font-weight: 800;
            color: var(--accent-light);
            letter-spacing: 2px;
        }

        nav a {
            color: var(--text-muted);
            text-decoration: none;
            margin-left: 24px;
            transition: color 0.2s;
        }

        nav a:hover {
            color: var(--accent-light);
        }

        .hero {
            text-align: center;
            padding: 80px 0 60px;
        }

        .hero h1 {
            font-size: clamp(2.5rem, 6vw, 4rem);
            margin-bottom: 16px;
            background: linear-gradient(135deg, var(--accent-light), #c084fc);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.2rem;
            color: var(--text-muted);
            max-width: 700px;
            margin: 0 auto 32px;
        }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 24px;
            margin-bottom: 80px;
        }

        .feature-card {
            background: var(--card);
            border: 1px solid var(--border);
            border-radius: 16px;
            padding: 28px;
            transition: transform 0.3s, border-color 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-4px);
            border-color: var(--accent);
        }

        .feature-card h3 {
            color: var(--accent-light);
            margin-bottom: 12px;
            font-size: 1.1rem;
        }

        .feature-card p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .section-title {
            font-size: 1.8rem;
            margin: 60px 0 24px;
            text-align: center;
        }

        .prompts-section {
            background: var(--bg-alt);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 60px;
        }

        .prompt-block {
            background: var(--bg);
            border: 1px solid var(--border);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 20px;
        }

        .prompt-block h4 {
            color: var(--accent-light);
            margin-bottom: 10px;
        }

        pre {
            background: #0f0f16;
            padding: 14px;
            border-radius: 8px;
            overflow-x: auto;
            font-size: 0.88rem;
            color: #a5f3fc;
            white-space: pre-wrap;
        }

        .copy-btn {
            background: var(--accent);
            color: white;
            border: none;
            padding: 6px 14px;
            border-radius: 6px;
            margin-top: 10px;
            cursor: pointer;
            font-size: 0.85rem;
            transition: background 0.2s;
        }

        .copy-btn:hover {
            background: var(--accent-light);
        }

        .login-box {
            max-width: 420px;
            margin: 40px auto 80px;
            background: var(--card);
            border: 1px solid var(--border);
            border-radius: 16px;
            padding: 36px;
            text-align: center;
        }

        .login-box h2 {
            margin-bottom: 24px;
            color: var(--accent-light);
        }

        input {
            width: 100%;
            padding: 12px 16px;
            background: var(--bg);
            border: 1px solid var(--border);
            border-radius: 8px;
            color: var(--text);
            font-size: 1rem;
            margin-bottom: 16px;
        }

        button.primary {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, var(--accent), var(--accent-light));
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: opacity 0.2s;
        }

        button.primary:hover {
            opacity: 0.9;
        }

        footer {
            text-align: center;
            padding: 30px;
            border-top: 1px solid var(--border);
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            .prompts-section { padding: 24px; }
            nav a { margin-left: 12px; font-size: 0.9rem; }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">WESIA</div>
            <nav>
                <a href="#recursos">Recursos</a>
                <a href="#prompts">Prompts</a>
                <a href="#acesso">Acesso</a>
            </nav>
        </header>

        <section class="hero">
            <h1>Seu Estúdio Inteligente</h1>
            <p>Converse, pesquise, programe, crie imagens, vídeos e sites — tudo em um só espaço. Simples, inteligente e feito para você.</p>
        </section>

        <h2 class="section-title" id="recursos">✨ Recursos Aprimorados</h2>
        <section class="features">
            <div class="feature-card">
                <h3>🧠 Mais Inteligente</h3>
                <p>Memória de projeto, compreensão de intenção e sugestões automáticas. A Wesia entende o que você quer criar.</p>
            </div>
            <div class="feature-card">
                <h3>🔍 Pesquisa Inteligente</h3>
                <p>Busca semântica em tempo real, filtros inteligentes e resumos organizados. Encontre inspirações e referências com facilidade.</p>
            </div>
            <div class="feature-card">
                <h3>🎬 Criação & Edição de Vídeo</h3>
                <p>Gere vídeos do zero por texto, edite com comandos simples, adicione legendas automáticas e exporte em qualquer formato.</p>
            </div>
            <div class="feature-card">
                <h3>🌐 Criação de Sites</h3>
                <p>Descreva o que você precisa e ganhe um site completo, responsivo e otimizado. Edite por conversa — sem código necessário.</p>
            </div>
        </section>

        <h2 class="section-title" id="prompts">📋 Guia de Prompts Prontos</h2>
        <section class="prompts-section">
            <div class="prompt-block">
                <h4>🧠 Fórmula Geral</h4>
                <pre id="p1">[PAPEL] + [CONTEXTO] + [OBJETIVO] + [ESTILO] + [FORMATO DE SAÍDA] + [O QUE EVITAR]</pre>
                <button class="copy-btn" onclick="copiar('p1')">Copiar</button>
            </div>

            <div class="prompt-block">
                <h4>🔍 Pesquisa</h4>
                <pre id="p2">Pesquise sobre: [tema]
Foque em: [tendências / exemplos / dados / inspirações visuais]
Período: [atual / últimos meses]
Organize por: [tópicos / prós e contras / exemplos práticos]
Destaque o que é mais útil para criação de conteúdo.</pre>
                <button class="copy-btn" onclick="copiar('p2')">Copiar</button>
            </div>

            <div class="prompt-block">
                <h4>🎬 Criar Vídeo do Zero</h4>
                <pre id="p3">Crie um vídeo de [duração] segundos sobre [assunto].
Estilo: [cinemático / dinâmico / minimalista]
Tom: [inspirador / informativo / energético]
Música: [animada / suave / sem música]
Legendas: [sim/não, cor e fonte]
Formato: [vertical 9:16 / horizontal 16:9 / quadrado 1:1]</pre>
                <button class="copy-btn" onclick="copiar('p3')">Copiar</button>
            </div>

            <div class="prompt-block">
                <h4>✂️ Editar Vídeo Existente</h4>
                <pre id="p4">Edite este vídeo:
- Duração alvo: [XX segundos]
- Remova partes silenciosas
- Adicione legendas claras e sincronizadas
- Ajuste brilho e contraste
- Deixe mais dinâmico nos primeiros 3 segundos
- Saída: formato para TikTok/Reels/YouTube</pre>
                <button class="copy-btn" onclick="copiar('p4')">Copiar</button>
            </div>

            <div class="prompt-block">
                <h4>🌐 Criar Site Completo</h4>
                <pre id="p5">Crie um site para [seu ramo/objetivo].
Páginas: [início, sobre, serviços, portfólio, contato]
Estilo: [moderno / minimalista / criativo / profissional]
Cores: [branco, cinza escuro, detalhes em azul]
Público-alvo: [quem visita]
Prioridade: [velocidade / visual / funcionalidade]
Inclua: formulário, redes sociais, seção de destaque.</pre>
                <button class="copy-btn" onclick="copiar('p5')">Copiar</button>
            </div>

            <div class="prompt-block">
                <h4>🔧 Ajustar Site Existente</h4>
                <pre id="p6">Atualize este site:
- Destaque o principal na página inicial
- Simplifique o menu
- Adicione seção de perguntas frequentes
- Otimize para celular
- Troque fontes por algo mais limpo</pre>
                <button class="copy-btn" onclick="copiar('p6')">Copiar</button>
            </div>
        </section>

        <h2 class="section-title" id="acesso">🔐 Acesso ao Estúdio</h2>
        <section class="login-box">
            <h2>Bem-vindo à WESIA</h2>
            <input type="text" placeholder="Usuário" value="WESIA-ADMIN">
            <input type="password" placeholder="Senha">
            <button class="primary">Acessar meu estúdio →</button>
        </section>
    </div>

    <footer>
        <p>Wesia — Seu Estúdio Inteligente de IA © 2026</p>
        <p style="margin-top: 8px; font-size: 0.8rem;">Converse · Pesquise · Crie · Edite · Publique</p>
    </footer>

    <script>
        function copiar(id) {
            const texto = document.getElementById(id).textContent;
            navigator.clipboard.writeText(texto).then(() => {
                const btn = event.target;
                const original = btn.textContent;
                btn.textContent = '✓ Copiado!';
                btn.style.background = '#10b981';
                setTimeout(() => {
                    btn.textContent = original;
                    btn.style.background = '';
                }, 2000);
            });
        }
    </script>
</body>
</html>
