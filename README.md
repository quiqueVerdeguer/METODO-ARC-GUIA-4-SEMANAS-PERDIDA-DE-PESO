<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Guía Regalo: Pierde 4 kg de Grasa en Solo 4 Semanas</title>
    <style>
        body {
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('/mnt/data/3668.JPEG');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
            min-height: 100%;
            position: relative;
            overflow-x: hidden;
        }
        
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 80%, rgba(120, 119, 198, 0.2) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 119, 198, 0.2) 0%, transparent 50%),
                linear-gradient(135deg, rgba(102, 126, 234, 0.3) 0%, rgba(118, 75, 162, 0.3) 100%);
            z-index: -1;
            animation: float 20s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }
        
        html {
            height: 100%;
        }
        
        .document-container {
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
            min-height: 100%;
            position: relative;
            z-index: 1;
        }
        
        .page {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
            border-radius: 15px;
            overflow: hidden;
            margin-bottom: 20px;
            min-height: 80vh;
            display: none;
            position: relative;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .page.active {
            display: block;
        }
        
        .page-header {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 30px;
            text-align: center;
            position: relative;
            box-shadow: 0 4px 20px rgba(255, 107, 107, 0.3);
        }
        
        .page-number {
            position: absolute;
            top: 15px;
            right: 20px;
            background: rgba(255,255,255,0.2);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
        }
        
        .page-title {
            font-size: 2rem;
            margin: 0;
            font-weight: 700;
            text-shadow: 0 2px 4px rgba(0,0,0,0.2);
        }
        
        .page-subtitle {
            font-size: 1.1rem;
            margin: 10px 0 0 0;
            opacity: 0.9;
        }
        
        .page-content {
            padding: 40px;
            min-height: 60vh;
            position: relative;
        }
        
        .instagram-handle {
            position: absolute;
            bottom: 20px;
            left: 20px;
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            display: flex;
            align-items: center;
            gap: 5px;
            z-index: 10;
        }
        
        .navigation {
            position: fixed;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(255,255,255,0.95);
            backdrop-filter: blur(15px);
            border-radius: 50px;
            padding: 15px 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            display: flex;
            gap: 15px;
            align-items: center;
            z-index: 1000;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .nav-btn {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 25px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            font-size: 0.9rem;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
        }
        
        .nav-btn:hover {
            background: linear-gradient(135deg, #ee5a24, #d63031);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(255, 107, 107, 0.4);
        }
        
        .nav-btn:disabled {
            background: #ccc;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
        }
        
        .page-indicator {
            display: flex;
            gap: 8px;
            margin: 0 10px;
        }
        
        .dot {
            width: 8px;
            height: 8px;
            border-radius: 50%;
            background: #ddd;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .dot.active {
            background: #ff6b6b;
            transform: scale(1.2);
            box-shadow: 0 2px 8px rgba(255, 107, 107, 0.4);
        }
        
        .table-of-contents {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .toc-item {
            background: linear-gradient(135deg, rgba(248,249,250,0.9), rgba(233,236,239,0.9));
            backdrop-filter: blur(10px);
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #ff6b6b;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .toc-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.15);
            background: linear-gradient(135deg, rgba(255,255,255,0.95), rgba(248,249,250,0.95));
        }
        
        .toc-number {
            font-size: 2rem;
            font-weight: 800;
            color: #ff6b6b;
            margin-bottom: 10px;
            text-shadow: 0 2px 4px rgba(255, 107, 107, 0.2);
        }
        
        .toc-title {
            font-size: 1.1rem;
            font-weight: 600;
            color: #2c3e50;
            margin: 0;
        }
        
        .section {
            margin-bottom: 40px;
            background: rgba(248,249,250,0.8);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 30px;
            border-left: 5px solid #ff6b6b;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .section h2 {
            color: #2c3e50;
            font-size: 1.8rem;
            margin: 0 0 20px 0;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .tip {
            background: rgba(255,255,255,0.9);
            backdrop-filter: blur(10px);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border-left: 4px solid #ff6b6b;
            border: 1px solid rgba(255, 255, 255, 0.3);
            transition: all 0.3s ease;
        }
        
        .tip:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }
        
        .tip h3 {
            color: #ff6b6b;
            margin: 0 0 10px 0;
            font-size: 1.1rem;
        }
        
        .foods-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }
        
        .food-item {
            background: rgba(255,255,255,0.9);
            backdrop-filter: blur(10px);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .food-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
        }
        
        .food-emoji {
            font-size: 2rem;
            margin-bottom: 10px;
        }
        
        .calculator {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
        }
        
        .calc-inputs {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .input-group {
            text-align: left;
        }
        
        .input-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
        }
        
        .input-group input, .input-group select {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            box-sizing: border-box;
            background: rgba(255,255,255,0.95);
            backdrop-filter: blur(10px);
        }
        
        .calc-button {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 25px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin: 20px 0;
            box-shadow: 0 6px 20px rgba(255, 107, 107, 0.3);
        }
        
        .calc-button:hover {
            background: linear-gradient(135deg, #ee5a24, #d63031);
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
        }
        
        .result {
            background: rgba(255,255,255,0.2);
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .diet-example {
            background: rgba(255,255,255,0.9);
            backdrop-filter: blur(10px);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .meal {
            padding: 20px;
            border-bottom: 1px solid rgba(238, 238, 238, 0.5);
        }
        
        .meal:last-child {
            border-bottom: none;
        }
        
        .meal h4 {
            color: #ff6b6b;
            margin: 0 0 10px 0;
            font-size: 1.2rem;
        }
        
        .footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 30px;
        }
        
        .footer h3 {
            margin: 0 0 10px 0;
            color: #ff6b6b;
        }
        
        @media (max-width: 768px) {
            .document-container {
                margin: 10px;
                padding: 15px;
            }
            
            .page-header {
                padding: 25px 20px;
            }
            
            .page-title {
                font-size: 1.7rem;
            }
            
            .page-content {
                padding: 25px 20px;
            }
            
            .navigation {
                bottom: 20px;
                padding: 12px 20px;
            }
            
            .nav-btn {
                padding: 10px 16px;
                font-size: 0.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="document-container">
        <!-- Página 1: Portada e Índice -->
        <div class="page active" id="page-1">
            <div class="page-header">
                <div class="page-number">Página 1 de 7</div>
                <h1 class="page-title">🔥 Pierde 4 kg de Grasa</h1>
                <p class="page-subtitle">en Solo 4 Semanas - Guía Completa</p>
            </div>
            <div class="page-content">
                <div style="background: linear-gradient(135deg, #4ecdc4, #44a08d); color: white; border-radius: 15px; padding: 30px; text-align: center; margin-bottom: 30px; box-shadow: 0 10px 30px rgba(78, 205, 196, 0.3);">
                    <h2 style="color: white; margin: 0 0 20px 0; font-size: 1.8rem;">🎉 ¡Gracias por descargar esta guía gratuita!</h2>
                    <p style="font-size: 1.1rem; margin-bottom: 25px; line-height: 1.6;">
                        Aquí encontrarás todo lo que necesitas para comenzar a perder grasa de forma efectiva y saludable.
                    </p>
                    
                    <div style="background: rgba(255,255,255,0.2); border-radius: 10px; padding: 25px; margin: 20px 0; backdrop-filter: blur(10px);">
                        <h3 style="color: white; margin: 0 0 15px 0; font-size: 1.3rem;">¿Qué vas a aprender?</h3>
                        <div style="text-align: left; display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px;">
                            <div style="display: flex; align-items: center; gap: 10px;">
                                <span style="color: #4ecdc4; font-size: 1.2rem;">✅</span>
                                <span>Cómo generar un déficit calórico sin pasar hambre</span>
                            </div>
                            <div style="display: flex; align-items: center; gap: 10px;">
                                <span style="color: #4ecdc4; font-size: 1.2rem;">✅</span>
                                <span>Qué alimentos aceleran tu proceso</span>
                            </div>
                            <div style="display: flex; align-items: center; gap: 10px;">
                                <span style="color: #4ecdc4; font-size: 1.2rem;">✅</span>
                                <span>Qué ejercicios y hábitos sí funcionan</span>
                            </div>
                            <div style="display: flex; align-items: center; gap: 10px;">
                                <span style="color: #4ecdc4; font-size: 1.2rem;">✅</span>
                                <span>Cómo adaptar una dieta a tu caso</span>
                            </div>
                        </div>
                    </div>
                    
                    <p style="font-size: 1.2rem; font-weight: 600; margin: 20px 0 0 0;">
                        🚀 Este es tu primer paso hacia un nuevo estilo de vida. ¡Vamos a por ello!
                    </p>
                </div>
                
                <h2 style="text-align: center; color: #2c3e50; margin: 30px 0 20px 0;">📋 Índice de Contenidos</h2>
                <div class="table-of-contents">
                    <div class="toc-item" onclick="goToPage(2)">
                        <div class="toc-number">1</div>
                        <h3 class="toc-title">10 Consejos para Perder Grasa</h3>
                    </div>
                    <div class="toc-item" onclick="goToPage(3)">
                        <div class="toc-number">2</div>
                        <h3 class="toc-title">Alimentos Recomendados</h3>
                    </div>
                    <div class="toc-item" onclick="goToPage(4)">
                        <div class="toc-number">3</div>
                        <h3 class="toc-title">Pautas de Nutrición</h3>
                    </div>
                    <div class="toc-item" onclick="goToPage(5)">
                        <div class="toc-number">4</div>
                        <h3 class="toc-title">Ejemplo de Dieta</h3>
                    </div>
                    <div class="toc-item" onclick="goToPage(6)">
                        <div class="toc-number">5</div>
                        <h3 class="toc-title">Calculadora ARC</h3>
                    </div>
                    <div class="toc-item" onclick="goToPage(7)">
                        <div class="toc-number">6</div>
                        <h3 class="toc-title">Conclusión</h3>
                    </div>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>
            
        <!-- Página 2: 10 Consejos -->
        <div class="page" id="page-2">
            <div class="page-header">
                <div class="page-number">Página 2 de 7</div>
                <h1 class="page-title">💡 10 Consejos Clave</h1>
                <p class="page-subtitle">para Perder Grasa de Forma Efectiva</p>
            </div>
            <div class="page-content">
                <div class="tips-grid">
                    <div class="tip">
                        <h3>1. Déficit Calórico Moderado</h3>
                        <p>Consume 300-500 calorías menos de las que quemas diariamente para una pérdida sostenible.</p>
                    </div>
                    <div class="tip">
                        <h3>2. Prioriza las Proteínas</h3>
                        <p>Consume 1.6-2.2g de proteína por kg de peso corporal para mantener masa muscular.</p>
                    </div>
                    <div class="tip">
                        <h3>3. Hidratación Constante</h3>
                        <p>Bebe al menos 2-3 litros de agua al día para optimizar el metabolismo.</p>
                    </div>
                    <div class="tip">
                        <h3>4. Ejercicio de Fuerza</h3>
                        <p>Entrena con pesas 3-4 veces por semana para preservar músculo durante la pérdida de peso.</p>
                    </div>
                    <div class="tip">
                        <h3>5. Cardio Inteligente</h3>
                        <p>Combina HIIT (2-3 veces) con cardio moderado (2-3 veces) por semana.</p>
                    </div>
                    <div class="tip">
                        <h3>6. Descanso de Calidad</h3>
                        <p>Duerme 7-9 horas diarias para regular hormonas del hambre y recuperación.</p>
                    </div>
                    <div class="tip">
                        <h3>7. Comidas Frecuentes</h3>
                        <p>Realiza 4-5 comidas pequeñas al día para mantener el metabolismo activo.</p>
                    </div>
                    <div class="tip">
                        <h3>8. Fibra en Cada Comida</h3>
                        <p>Incluye vegetales y frutas para aumentar saciedad y mejorar digestión.</p>
                    </div>
                    <div class="tip">
                        <h3>9. Grasas Saludables</h3>
                        <p>Consume aguacate, frutos secos y aceite de oliva con moderación.</p>
                    </div>
                    <div class="tip">
                        <h3>10. Consistencia Total</h3>
                        <p>Mantén el plan 6 días a la semana, permite 1 día de flexibilidad controlada.</p>
                    </div>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>

        <!-- Página 3: Alimentos Recomendados -->
        <div class="page" id="page-3">
            <div class="page-header">
                <div class="page-number">Página 3 de 7</div>
                <h1 class="page-title">🥗 Alimentos Recomendados</h1>
                <p class="page-subtitle">Los mejores alimentos para acelerar tu pérdida de grasa</p>
            </div>
            <div class="page-content">
                <div class="foods-grid">
                    <div class="food-item">
                        <div class="food-emoji">🐟</div>
                        <strong>Proteínas Magras</strong>
                        <p>Pollo, pescado, huevos, tofu</p>
                    </div>
                    <div class="food-item">
                        <div class="food-emoji">🥬</div>
                        <strong>Vegetales Verdes</strong>
                        <p>Espinacas, brócoli, apio, pepino</p>
                    </div>
                    <div class="food-item">
                        <div class="food-emoji">🍓</div>
                        <strong>Frutas Bajas en Azúcar</strong>
                        <p>Fresas, arándanos, manzana verde</p>
                    </div>
                    <div class="food-item">
                        <div class="food-emoji">🌾</div>
                        <strong>Carbohidratos Complejos</strong>
                        <p>Avena, quinoa, batata, arroz integral</p>
                    </div>
                    <div class="food-item">
                        <div class="food-emoji">🥑</div>
                        <strong>Grasas Saludables</strong>
                        <p>Aguacate, almendras, aceite de oliva</p>
                    </div>
                    <div class="food-item">
                        <div class="food-emoji">💧</div>
                        <strong>Hidratación</strong>
                        <p>Agua, té verde, infusiones naturales</p>
                    </div>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>

        <!-- Página 4: Pautas de Nutrición -->
        <div class="page" id="page-4">
            <div class="page-header">
                <div class="page-number">Página 4 de 7</div>
                <h1 class="page-title">📊 Pautas de Nutrición</h1>
                <p class="page-subtitle">Guías esenciales para optimizar tu alimentación</p>
            </div>
            <div class="page-content">
                <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
                    <div style="background: rgba(255,255,255,0.9); backdrop-filter: blur(10px); padding: 25px; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); border-left: 4px solid #4ecdc4; border: 1px solid rgba(255, 255, 255, 0.3);">
                        <h3 style="color: #4ecdc4; margin: 0 0 15px 0; font-size: 1.2rem;">⚖️ Distribución de Macronutrientes</h3>
                        <ul style="margin: 0; padding-left: 20px; line-height: 1.6;">
                            <li><strong>Proteínas:</strong> 25-30% del total calórico</li>
                            <li><strong>Carbohidratos:</strong> 35-40% del total calórico</li>
                            <li><strong>Grasas:</strong> 25-30% del total calórico</li>
                        </ul>
                    </div>
                    <div style="background: rgba(255,255,255,0.9); backdrop-filter: blur(10px); padding: 25px; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); border-left: 4px solid #ff6b6b; border: 1px solid rgba(255, 255, 255, 0.3);">
                        <h3 style="color: #ff6b6b; margin: 0 0 15px 0; font-size: 1.2rem;">🕐 Timing de Comidas</h3>
                        <ul style="margin: 0; padding-left: 20px; line-height: 1.6;">
                            <li>Desayuno: 25% de calorías diarias</li>
                            <li>Almuerzo: 35% de calorías diarias</li>
                            <li>Cena: 25% de calorías diarias</li>
                            <li>Snacks: 15% de calorías diarias</li>
                        </ul>
                    </div>
                    <div style="background: rgba(255,255,255,0.9); backdrop-filter: blur(10px); padding: 25px; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); border-left: 4px solid #44a08d; border: 1px solid rgba(255, 255, 255, 0.3);">
                        <h3 style="color: #44a08d; margin: 0 0 15px 0; font-size: 1.2rem;">💧 Hidratación Óptima</h3>
                        <ul style="margin: 0; padding-left: 20px; line-height: 1.6;">
                            <li>Al despertar: 500ml de agua</li>
                            <li>Antes de comidas: 250ml</li>
                            <li>Durante ejercicio: 150-200ml cada 15-20min</li>
                            <li>Total diario: 35ml por kg de peso</li>
                        </ul>
                    </div>
                    <div style="background: rgba(255,255,255,0.9); backdrop-filter: blur(10px); padding: 25px; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); border-left: 4px solid #764ba2; border: 1px solid rgba(255, 255, 255, 0.3);">
                        <h3 style="color: #764ba2; margin: 0 0 15px 0; font-size: 1.2rem;">🚫 Alimentos a Evitar</h3>
                        <ul style="margin: 0; padding-left: 20px; line-height: 1.6;">
                            <li>Azúcares refinados y dulces procesados</li>
                            <li>Bebidas azucaradas y alcohol</li>
                            <li>Frituras y comida rápida</li>
                            <li>Harinas blancas y productos ultraprocesados</li>
                        </ul>
                    </div>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>

        <!-- Página 5: Ejemplo de Dieta -->
        <div class="page" id="page-5">
            <div class="page-header">
                <div class="page-number">Página 5 de 7</div>
                <h1 class="page-title">📋 Ejemplo de Dieta</h1>
                <p class="page-subtitle">Plan alimentario diario completo</p>
            </div>
            <div class="page-content">
                <div class="diet-example">
                    <div class="meal">
                        <h4>🌅 Desayuno (7:00 AM)</h4>
                        <p><strong>Opción 1:</strong> 3 claras + 1 huevo entero, 40g avena, 1 taza de fresas</p>
                        <p><strong>Opción 2:</strong> Batido de proteína con 1 plátano y espinacas</p>
                    </div>
                    <div class="meal">
                        <h4>🍎 Media Mañana (10:00 AM)</h4>
                        <p>1 manzana verde + 15 almendras</p>
                    </div>
                    <div class="meal">
                        <h4>🍽️ Almuerzo (13:00 PM)</h4>
                        <p>150g pechuga de pollo, 100g arroz integral, ensalada mixta con aceite de oliva</p>
                    </div>
                    <div class="meal">
                        <h4>🥤 Merienda (16:00 PM)</h4>
                        <p>Yogur griego natural + 1 cucharada de chía</p>
                    </div>
                    <div class="meal">
                        <h4>🌙 Cena (19:00 PM)</h4>
                        <p>150g pescado blanco, 200g vegetales al vapor, 1/2 aguacate</p>
                    </div>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>

        <!-- Página 6: Calculadora ARC -->
        <div class="page" id="page-6">
            <div class="page-header">
                <div class="page-number">Página 6 de 7</div>
                <h1 class="page-title">🧮 Calculadora ARC</h1>
                <p class="page-subtitle">Calcula tu plan personalizado</p>
            </div>
            <div class="page-content">
                <div class="calculator">
                    <p style="color: white; font-size: 1.1rem; margin-bottom: 20px;">Calcula tus necesidades calóricas para perder 4kg en 4 semanas</p>
                    
                    <form class="calc-inputs" onsubmit="calculateCalories(event)">
                        <div class="input-group">
                            <label for="weight">Peso actual (kg)</label>
                            <input type="number" id="weight" required min="40" max="200">
                        </div>
                        <div class="input-group">
                            <label for="height">Altura (cm)</label>
                            <input type="number" id="height" required min="140" max="220">
                        </div>
                        <div class="input-group">
                            <label for="age">Edad (años)</label>
                            <input type="number" id="age" required min="18" max="80">
                        </div>
                        <div class="input-group">
                            <label for="gender">Género</label>
                            <select id="gender" required>
                                <option value="">Seleccionar</option>
                                <option value="male">Masculino</option>
                                <option value="female">Femenino</option>
                            </select>
                        </div>
                        <div class="input-group">
                            <label for="activity">Nivel de Actividad</label>
                            <select id="activity" required>
                                <option value="">Seleccionar</option>
                                <option value="1.2">Sedentario</option>
                                <option value="1.375">Ligero (1-3 días/semana)</option>
                                <option value="1.55">Moderado (3-5 días/semana)</option>
                                <option value="1.725">Activo (6-7 días/semana)</option>
                                <option value="1.9">Muy activo (2 veces/día)</option>
                            </select>
                        </div>
                    </form>
                    
                    <button type="submit" class="calc-button" onclick="calculateCalories(event)">
                        Calcular Mi Plan Personalizado
                    </button>
                    
                    <div id="result" class="result" style="display: none;">
                        <h3>📊 Tu Plan Personalizado</h3>
                        <div id="resultContent"></div>
                    </div>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>

        <!-- Página 7: Conclusión -->
        <div class="page" id="page-7">
            <div class="page-header">
                <div class="page-number">Página 7 de 7</div>
                <h1 class="page-title">🎯 Conclusión</h1>
                <p class="page-subtitle">Tu camino hacia el éxito</p>
            </div>
            <div class="page-content">
                <div style="background: linear-gradient(135deg, #667eea, #764ba2); color: white; border-radius: 15px; padding: 40px; text-align: center; box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);">
                    <div style="background: rgba(255,255,255,0.1); border-radius: 10px; padding: 30px; margin: 25px 0; backdrop-filter: blur(10px);">
                        <p style="font-size: 1.2rem; line-height: 1.7; margin-bottom: 20px;">
                            Perder 4kg de grasa en 4 semanas es un objetivo <strong>realista y alcanzable</strong> cuando sigues un plan estructurado y basado en evidencia científica.
                        </p>
                        
                        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 25px 0; text-align: left;">
                            <div style="background: rgba(255,255,255,0.1); padding: 20px; border-radius: 8px;">
                                <h4 style="color: #4ecdc4; margin: 0 0 10px 0;">🔑 Claves del Éxito</h4>
                                <ul style="margin: 0; padding-left: 20px; line-height: 1.6;">
                                    <li>Consistencia en la alimentación</li>
                                    <li>Ejercicio regular y progresivo</li>
                                    <li>Descanso de calidad</li>
                                    <li>Hidratación adecuada</li>
                                </ul>
                            </div>
                            <div style="background: rgba(255,255,255,0.1); padding: 20px; border-radius: 8px;">
                                <h4 style="color: #ff6b6b; margin: 0 0 10px 0;">⚠️ Recuerda</h4>
                                <ul style="margin: 0; padding-left: 20px; line-height: 1.6;">
                                    <li>Los resultados varían por persona</li>
                                    <li>La paciencia es fundamental</li>
                                    <li>Consulta a un profesional si es necesario</li>
                                    <li>Escucha a tu cuerpo</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                    <div style="background: rgba(255,255,255,0.2); border-radius: 10px; padding: 25px; margin: 25px 0;">
                        <h3 style="color: white; margin: 0 0 15px 0; font-size: 1.4rem;">🚀 Tu Próximo Paso</h3>
                        <p style="font-size: 1.1rem; line-height: 1.6; margin: 0;">
                            Utiliza la <strong>Calculadora ARC</strong> para obtener tu plan personalizado y comienza <strong>HOY MISMO</strong>. 
                            Recuerda que cada día que esperas es un día menos para alcanzar tus objetivos.
                        </p>
                    </div>
                    
                    <p style="font-size: 1.3rem; font-weight: 700; margin: 30px 0 0 0; color: #4ecdc4;">
                        💪 ¡Tu mejor versión te está esperando!
                    </p>
                </div>
                <div class="instagram-handle">
                    📸 @QUIQUE_VERDEGUER
                </div>
            </div>
        </div>

        <!-- Navegación -->
        <div class="navigation">
            <button class="nav-btn" onclick="previousPage()" id="prevBtn">← Anterior</button>
            <div class="page-indicator">
                <div class="dot active" onclick="goToPage(1)"></div>
                <div class="dot" onclick="goToPage(2)"></div>
                <div class="dot" onclick="goToPage(3)"></div>
                <div class="dot" onclick="goToPage(4)"></div>
                <div class="dot" onclick="goToPage(5)"></div>
                <div class="dot" onclick="goToPage(6)"></div>
                <div class="dot" onclick="goToPage(7)"></div>
            </div>
            <button class="nav-btn" onclick="nextPage()" id="nextBtn">Siguiente →</button>
        </div>
    </div>

    <script>
        let currentPage = 1;
        const totalPages = 7;
        
        function showPage(pageNumber) {
            // Ocultar todas las páginas
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            
            // Mostrar la página seleccionada
            document.getElementById(`page-${pageNumber}`).classList.add('active');
            
            // Actualizar indicadores
            document.querySelectorAll('.dot').forEach((dot, index) => {
                dot.classList.toggle('active', index + 1 === pageNumber);
            });
            
            // Actualizar botones de navegación
            document.getElementById('prevBtn').disabled = pageNumber === 1;
            document.getElementById('nextBtn').disabled = pageNumber === totalPages;
            
            currentPage = pageNumber;
            
            // Scroll al inicio de la página
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }
        
        function goToPage(pageNumber) {
            if (pageNumber >= 1 && pageNumber <= totalPages) {
                showPage(pageNumber);
            }
        }
        
        function nextPage() {
            if (currentPage < totalPages) {
                goToPage(currentPage + 1);
            }
        }
        
        function previousPage() {
            if (currentPage > 1) {
                goToPage(currentPage - 1);
            }
        }
        
        // Navegación con teclado
        document.addEventListener('keydown', function(event) {
            if (event.key === 'ArrowRight' || event.key === ' ') {
                event.preventDefault();
                nextPage();
            } else if (event.key === 'ArrowLeft') {
                event.preventDefault();
                previousPage();
            }
        });
        
        function calculateCalories(event) {
            event.preventDefault();
            
            const weight = parseFloat(document.getElementById('weight').value);
            const height = parseFloat(document.getElementById('height').value);
            const age = parseFloat(document.getElementById('age').value);
            const gender = document.getElementById('gender').value;
            const activity = parseFloat(document.getElementById('activity').value);
            
            if (!weight || !height || !age || !gender || !activity) {
                // Crear mensaje personalizado en lugar de alert
                const message = document.createElement('div');
                message.style.cssText = `
                    position: fixed;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    background: linear-gradient(135deg, #ff6b6b, #ee5a24);
                    color: white;
                    padding: 20px 30px;
                    border-radius: 15px;
                    box-shadow: 0 15px 35px rgba(255, 107, 107, 0.4);
                    z-index: 10000;
                    font-weight: 600;
                    backdrop-filter: blur(10px);
                    border: 1px solid rgba(255, 255, 255, 0.2);
                `;
                message.textContent = 'Por favor, completa todos los campos';
                document.body.appendChild(message);
                
                setTimeout(() => {
                    document.body.removeChild(message);
                }, 3000);
                return;
            }
            
            // Calcular BMR usando la fórmula de Mifflin-St Jeor
            let bmr;
            if (gender === 'male') {
                bmr = (10 * weight) + (6.25 * height) - (5 * age) + 5;
            } else {
                bmr = (10 * weight) + (6.25 * height) - (5 * age) - 161;
            }
            
            // Calcular TDEE (Total Daily Energy Expenditure)
            const tdee = bmr * activity;
            
            // Para perder 4kg en 4 semanas necesitamos un déficit de 1000 cal/día
            // (4kg * 7700 cal/kg = 30800 cal / 28 días = 1100 cal/día)
            const targetCalories = Math.round(tdee - 1000);
            const protein = Math.round(weight * 2);
            const fat = Math.round(weight * 0.8);
            const carbs = Math.round((targetCalories - (protein * 4) - (fat * 9)) / 4);
            
            const resultDiv = document.getElementById('result');
            const resultContent = document.getElementById('resultContent');
            
            resultContent.innerHTML = `
                <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; text-align: center;">
                    <div>
                        <h4>🔥 Calorías Diarias</h4>
                        <p style="font-size: 2rem; font-weight: bold; color: #ff6b6b;">${targetCalories}</p>
                    </div>
                    <div>
                        <h4>🥩 Proteínas</h4>
                        <p style="font-size: 1.5rem; font-weight: bold;">${protein}g</p>
                    </div>
                    <div>
                        <h4>🍞 Carbohidratos</h4>
                        <p style="font-size: 1.5rem; font-weight: bold;">${carbs}g</p>
                    </div>
                    <div>
                        <h4>🥑 Grasas</h4>
                        <p style="font-size: 1.5rem; font-weight: bold;">${fat}g</p>
                    </div>
                </div>
                <div style="margin-top: 20px; padding: 15px; background: rgba(255,107,107,0.2); border-radius: 10px;">
                    <p><strong>💡 Recomendación:</strong> Sigue este plan junto con ejercicio regular para alcanzar tu objetivo de perder 4kg en 4 semanas de forma saludable.</p>
                </div>
            `;
            
            resultDiv.style.display = 'block';
            resultDiv.scrollIntoView({ behavior: 'smooth' });
        }
        
        // Inicializar la primera página
        document.addEventListener('DOMContentLoaded', function() {
            showPage(1);
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9956ae9e6748cfdf',t:'MTc2MTYxNTE3NS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
