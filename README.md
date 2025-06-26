<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Currículo - Ueliton Antônio de Oliveira</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --gray-color: #95a5a6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: #f9f9f9;
            padding: 20px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--dark-color));
            color: white;
            padding: 30px 40px;
            position: relative;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }
        
        .profile {
            display: flex;
            align-items: center;
        }
        
        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid white;
            margin-right: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .title h1 {
            font-size: 2.2rem;
            margin-bottom: 5px;
            font-weight: 700;
        }
        
        .title h2 {
            font-size: 1.3rem;
            font-weight: 400;
            opacity: 0.9;
        }
        
        .contact-info {
            text-align: right;
        }
        
        .contact-item {
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            justify-content: flex-end;
        }
        
        .contact-item i {
            margin-left: 10px;
            font-size: 1.1rem;
        }
        
        main {
            padding: 30px 40px;
        }
        
        section {
            margin-bottom: 30px;
        }
        
        .section-title {
            color: var(--primary-color);
            font-size: 1.5rem;
            margin-bottom: 15px;
            padding-bottom: 8px;
            border-bottom: 2px solid var(--secondary-color);
            display: flex;
            align-items: center;
        }
        
        .section-title i {
            margin-right: 10px;
            color: var(--secondary-color);
        }
        
        .section-content {
            padding-left: 20px;
        }
        
        .about p {
            margin-bottom: 15px;
            text-align: justify;
            line-height: 1.8;
        }
        
        .experience-item, .education-item {
            margin-bottom: 25px;
            position: relative;
            padding-left: 30px;
            border-left: 2px solid var(--light-color);
        }
        
        .experience-item:before, .education-item:before {
            content: '';
            position: absolute;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: var(--secondary-color);
            left: -7px;
            top: 5px;
        }
        
        .job-title, .degree {
            font-size: 1.2rem;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 5px;
        }
        
        .company, .institution {
            font-weight: 600;
            color: var(--primary-color);
            margin-bottom: 5px;
        }
        
        .date {
            color: var(--gray-color);
            font-size: 0.9rem;
            margin-bottom: 10px;
            display: block;
        }
        
        .job-description ul, .skills-list {
            list-style-type: none;
        }
        
        .job-description li {
            position: relative;
            padding-left: 20px;
            margin-bottom: 8px;
        }
        
        .job-description li:before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--secondary-color);
            font-weight: bold;
        }
        
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .skill-category {
            flex: 1;
            min-width: 250px;
        }
        
        .skill-category h3 {
            color: var(--primary-color);
            margin-bottom: 10px;
            font-size: 1.1rem;
        }
        
        .skills-list li {
            margin-bottom: 8px;
            display: flex;
            align-items: center;
        }
        
        .skills-list i {
            color: var(--secondary-color);
            margin-right: 8px;
            font-size: 0.8rem;
        }
        
        .languages-list {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .language-item {
            background: var(--light-color);
            padding: 10px 15px;
            border-radius: 5px;
            min-width: 150px;
        }
        
        .language-name {
            font-weight: 600;
            color: var(--primary-color);
        }
        
        .language-level {
            color: var(--gray-color);
            font-size: 0.9rem;
        }
        
        footer {
            background: var(--light-color);
            padding: 15px 40px;
            text-align: center;
            color: var(--gray-color);
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            .profile {
                flex-direction: column;
                margin-bottom: 20px;
            }
            
            .profile-img {
                margin-right: 0;
                margin-bottom: 15px;
            }
            
            .contact-info {
                text-align: center;
            }
            
            .contact-item {
                justify-content: center;
            }
            
            .skills-container {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="header-content">
                <div class="profile">
                    <!-- Imagem de perfil atualizada -->
                    <img src="profile.jpg" alt="Foto de Ueliton Antônio" class="profile-img">
                    <div class="title">
                        <h1>Ueliton Antônio de Oliveira</h1>
                        <h2>Mecânico Industrial Sênior | Líder Técnico</h2>
                    </div>
                </div>
                <div class="contact-info">
                    <div class="contact-item">
                        <span>(37) 99906-3862</span>
                        <i class="fas fa-phone"></i>
                    </div>
                    <div class="contact-item">
                        <span>ueliton833@gmail.com</span>
                        <i class="fas fa-envelope"></i>
                    </div>
                    <div class="contact-item">
                        <span>Lagoa da Prata, MG</span>
                        <i class="fas fa-map-marker-alt"></i>
                    </div>

                </div>
            </div>
        </header>
        
        <main>
            <section class="about">
                <h2 class="section-title"><i class="fas fa-user"></i> Perfil Profissional</h2>
                <div class="section-content">
                    <p>Profissional com mais de 8 anos de experiência em manutenção industrial, especializado em equipamentos de alta performance. Expertise em liderança de equipes multidisciplinares, análise de falhas mecânicas e implementação de processos de manutenção preventiva e preditiva.</p>
                    <p>Busco uma posição de Liderança em Manutenção Industrial onde possa aplicar minha experiência técnica e gerencial para otimizar processos, reduzir custos operacionais e aumentar a eficiência dos equipamentos.</p>
                </div>
            </section>
            
            <section class="experience">
                <h2 class="section-title"><i class="fas fa-briefcase"></i> Experiência Profissional</h2>
                <div class="section-content">
                    <div class="experience-item">
                        <h3 class="job-title">Mecânico Industrial Sênior</h3>
                        <span class="company">Raizen</span>
                        <span class="date">2017 - 2025 | Lagoa da Prata, MG</span>
                        <div class="job-description">
                            <ul>
                                <li>Liderança de equipes de até 15 técnicos em manutenções preventivas, preditivas e corretivas em equipamentos rotativos e estáticos.</li>
                                <li>Implementação de programa de manutenção preventiva que reduziu paradas não programadas em 35%.</li>
                                <li>Análise de falhas críticas utilizando metodologia RCFA (Root Cause Failure Analysis).</li>
                                <li>Coordenação de paradas técnicas programadas, garantindo cumprimento de prazos e orçamentos.</li>
                                <li>Padronização de procedimentos de manutenção alinhados às normas NR-12, ISO 9001 e 14001.</li>
                                <li>Treinamento e desenvolvimento de equipes técnicas multidisciplinares.</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="experience-item">
                        <h3 class="job-title">Mecânico Industrial Sênior</h3>
                        <span class="company">J.J Montagem e Manutenção</span>
                        <span class="date">2025 - Presente | São Paulo, SP</span>
                        <div class="job-description">
                            <ul>
                                <li>Montagem e alinhamento de equipamentos de alta precisão com tolerâncias abaixo de 0,05mm.</li>
                                <li>Diagnóstico e solução de problemas complexos em sistemas mecânicos e rotativos.</li>
                                <li>Elaboração de relatórios técnicos detalhados para clientes corporativos.</li>
                                <li>Consultoria técnica para projetos de instalação e modernização de equipamentos.</li>
                                <li>Utilização de tecnologias de alinhamento a laser e análise vibracional.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="education">
                <h2 class="section-title"><i class="fas fa-graduation-cap"></i> Formação Acadêmica</h2>
                <div class="section-content">
                    <div class="education-item">
                        <h3 class="degree">Técnico em Mecânica Industrial</h3>
                        <span class="institution">SENAI-MG</span>
                        <span class="date">2020 - 2021</span>
                    </div>
                    
                    <div class="education-item">
                        <h3 class="degree">Engenharia Química (incompleto)</h3>
                        <span class="institution">UNIFOR-MG</span>
                        <span class="date">2018 - 2020</span>
                    </div>
                </div>
            </section>
            
            <section class="skills">
                <h2 class="section-title"><i class="fas fa-cogs"></i> Habilidades Técnicas</h2>
                <div class="section-content">
                    <div class="skills-container">
                        <div class="skill-category">
                            <h3>Competências Técnicas</h3>
                            <ul class="skills-list">
                                <li><i class="fas fa-check"></i> Alinhamento de máquinas (laser e dial indicator)</li>
                                <li><i class="fas fa-check"></i> Análise de falhas (RCFA)</li>
                                <li><i class="fas fa-check"></i> Manutenção de bombas centrífugas e compressores</li>
                                <li><i class="fas fa-check"></i> Leitura e interpretação de desenhos técnicos</li>
                                <li><i class="fas fa-check"></i> Metrologia dimensional avançada</li>
                            </ul>
                        </div>
                        
                        <div class="skill-category">
                            <h3>Gestão e Liderança</h3>
                            <ul class="skills-list">
                                <li><i class="fas fa-check"></i> Gestão de equipes multidisciplinares</li>
                                <li><i class="fas fa-check"></i> Planejamento de manutenção</li>
                                <li><i class="fas fa-check"></i> Elaboração de KPIs e indicadores</li>
                                <li><i class="fas fa-check"></i> Gestão de custos e orçamentos</li>
                                <li><i class="fas fa-check"></i> Treinamento e desenvolvimento de equipes</li>
                            </ul>
                        </div>
                        
                        <div class="skill-category">
                            <h3>Ferramentas e Tecnologias</h3>
                            <ul class="skills-list">
                                <li><i class="fas fa-check"></i> Microsoft Office (Avançado)</li>
                                <li><i class="fas fa-check"></i> SAP PM (Módulo Manutenção)</li>
                                <li><i class="fas fa-check"></i> Softwares de alinhamento a laser</li>
                                <li><i class="fas fa-check"></i> AutoCAD básico</li>
                                <li><i class="fas fa-check"></i> Sistemas CMMS</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="languages">
                <h2 class="section-title"><i class="fas fa-language"></i> Idiomas</h2>
                <div class="section-content">
                    <div class="languages-list">
                        <div class="language-item">
                            <div class="language-name">Português</div>
                            <div class="language-level">Nativo</div>
                        </div>
                        <div class="language-item">
                            <div class="language-name">Inglês</div>
                            <div class="language-level">Intermediário (Técnico)</div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="certifications">
                <h2 class="section-title"><i class="fas fa-certificate"></i> Certificações</h2>
                <div class="section-content">
                    <ul class="skills-list">
                        <li><i class="fas fa-award"></i> NR-12 - Segurança no Trabalho em Máquinas e Equipamentos</li>
                        <li><i class="fas fa-award"></i> Alinhamento de Máquinas com Laser - SKF</li>
                        <li><i class="fas fa-award"></i> Análise de Vibração Nível I</li>
                        <li><i class="fas fa-award"></i> Gestão de Manutenção Produtiva (TPM)</li>
                    </ul>
                </div>
            </section>
            
            <section class="additional-info">
                <h2 class="section-title"><i class="fas fa-info-circle"></i> Informações Adicionais</h2>
                <div class="section-content">
                    <ul class="skills-list">
                        <li><i class="fas fa-passport"></i> Disponibilidade para viagens</li>
                        <li><i class="fas fa-user-tie"></i> Referências profissionais disponíveis sob solicitação</li>
                    </ul>
                </div>
            </section>
        </main>
        
        <footer>
            <p>Ueliton Antônio de Oliveira - © 2025 - Todos os direitos reservados</p>
        </footer>
    </div>
</body>
</html>
