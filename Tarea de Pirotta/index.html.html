<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Análisis Comparativo: Artes Multimediales</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/vis-network/9.1.2/dist/vis-network.min.js"></script>

    <style>
        body { font-family: 'Lexend', sans-serif; margin: 0; background: #08080a; color: #e0e0e0; overflow: hidden; }
        #network-container { width: 100vw; height: 100vh; }
        
        /* Menú de Línea de Tiempo */
        .timeline-sidebar { position: absolute; left: 20px; top: 50%; transform: translateY(-50%); 
            width: 200px; z-index: 10; border-left: 2px solid #333; padding-left: 20px; }

        .time-item { margin-bottom: 30px; position: relative; cursor: pointer; transition: 0.3s; }
        .time-item:hover { color: #00fbff; }

        .time-year { font-weight: bold; font-size: 18px; color: #00fbff; }
        .time-label { font-size: 12px; color: #888; }

        /* Panel */
        .info-panel { position: absolute; top: 20px; right: 20px; width: 380px; background: rgba(15,15,20,0.98);
            border: 1px solid #333; padding: 25px; border-radius: 15px; display: none; z-index: 20; }

        .info-panel h2 { color: #00fbff; }

        .index-box { background:#1a1a20; padding:10px; margin-top:10px; border-radius:8px; }

        .index-title { font-size:11px; color:#00fbff; }
        .index-value { font-size:14px; }

        .header-title { position: absolute; top: 20px; left: 20px; }

        /* ✅ SOLO AGREGADO */
        .map-index { 
            position: absolute; 
            bottom: 20px; 
            left: 20px; 
            background: rgba(20,20,25,0.9); 
            padding: 15px; 
            border-radius: 10px; 
            border: 1px solid #333; 
            font-size: 12px; 
            z-index: 10; 
        }

        .index-item { display: flex; align-items: center; margin-bottom: 5px; }
        .dot-index { width: 10px; height: 10px; border-radius: 50%; margin-right: 10px; }
    </style>
</head>

<body>

<div class="header-title">
    <h1>CARTOGRAFÍA CONCEPTUAL</h1>
</div>

<div class="timeline-sidebar">
    <div class="time-item" onclick="focusNode(1)">
        <span class="time-year">1999</span>
        <span class="time-label">Daniel Rozin</span>
    </div>
    <div class="time-item" onclick="focusNode(2)">
        <span class="time-year">2018</span>
        <span class="time-label">Ana Laura Cantera</span>
    </div>
    <div class="time-item" onclick="focusNode(3)">
        <span class="time-year">2018</span>
        <span class="time-label">Sandra de Berduccy</span>
    </div>
</div>

<!-- ✅ SOLO ESTO SE AGREGA -->
<div class="map-index">
    <div style="color:#00fbff; margin-bottom:10px;">ÍNDICE DEL MAPA</div>

    <div class="index-item">
        <div class="dot-index" style="background:#fff;"></div> Concepto Central
    </div>

    <div class="index-item">
        <div class="dot-index" style="background:#4a90e2;"></div> Eje Mecánico
    </div>

    <div class="index-item">
        <div class="dot-index" style="background:#7ed321;"></div> Eje Bioarte
    </div>

    <div class="index-item">
        <div class="dot-index" style="background:#f5a623;"></div> Eje Ancestral
    </div>

    <div class="index-item">
        <div class="dot-index" style="background:#ff4b5c;"></div> Usuario / Interacción
    </div>
</div>

<div id="info-panel" class="info-panel"></div>
<div id="network-container"></div>

<script>
const nodes = new vis.DataSet([
    { id: 0, label: 'ARTES\nMULTIMEDIALES', color: '#fff', size: 30, font: { size: 16, bold: true } },
    
    { id: 1, label: 'Daniel Rozin\n(Mecánico)', color: '#4a90e2', group: 'autor', 
      info: {
        title: "Daniel Rozin: El Reflejo Mecánico",
        contexto: "Fines del Siglo XX. Auge de la digitalización y robótica industrial.",
        hibridacion: "Alta. Traducción de imagen digital (software) a movimiento físico (madera/motores).",
        participacion: "Grado Máximo. El usuario es el motor activo del movimiento.",
        hipermedialidad: "Interactividad inmediata en tiempo real sin almacenamiento persistente."
      }
    },

    { id: 2, label: 'Ana Laura Cantera\n(Bioarte)', color: '#7ed321', group: 'autor',
      info: {
        title: "Ana Laura Cantera: Bio-Robótica",
        contexto: "Siglo XXI. Cruce de ciencia, biología y tecnología decolonial.",
        hibridacion: "Transdisciplinar. Cyborg híbrido: hongo vivo (cerebro) + máquina.",
        participacion: "Contemplativa. El usuario es parte del ecosistema pero no tiene control directo.",
        hipermedialidad: "Sistema de información vivo. Almacena y procesa datos ambientales."
      }
    },

    { id: 3, label: 'S. de Berduccy\n(Ancestral)', color: '#f5a623', group: 'autor',
      info: {
        title: "Sandra de Berduccy: Tejido-Circuito",
        contexto: "Contemporaneidad. Revalorización del telar como sistema binario.",
        hibridacion: "Binario-Textil. El hilo conductor es simultáneamente trama y cable.",
        participacion: "Ritual/Táctica. Requiere proximidad y energía electromagnética del cuerpo.",
        hipermedialidad: "Anticipación del código digital mediante tecnologías milenarias."
      }
    },

    { id: 100, label: 'USUARIO', shape: 'star', color: '#ff4b5c', size: 25 }
]);

const edges = new vis.DataSet([
    { from: 0, to: 1 }, { from: 0, to: 2 }, { from: 0, to: 3 },
    { from: 100, to: 1, label: 'INTERACCIÓN DIRECTA', dashes: [5,5], color: '#4a90e2' },
    { from: 100, to: 2, label: 'ECOSISTÉMICA', dashes: [5,5], color: '#7ed321' },
    { from: 100, to: 3, label: 'TACTO / RITUAL', dashes: [5,5], color: '#f5a623' }
]);

const network = new vis.Network(
    document.getElementById('network-container'),
    { nodes, edges },
    { physics:{ forceAtlas2Based:{ gravitationalConstant:-100 }, solver:'forceAtlas2Based' } }
);

const panel = document.getElementById('info-panel');

function focusNode(id) {
    network.focus(id, { scale: 1.2, animation: true });
    showInfo(id);
}

function showInfo(id) {
    const node = nodes.get(id);
    if (node && node.info) {
        panel.style.display = 'block';
        panel.innerHTML = `
            <h2>${node.info.title}</h2>
            <p><strong>Contexto:</strong> ${node.info.contexto}</p>
            
            <div class="index-box">
                <span class="index-title">Índice de Hibridación</span>
                <span class="index-value">${node.info.hibridacion}</span>
            </div>
            <div class="index-box">
                <span class="index-title">Grado de Participación</span>
                <span class="index-value">${node.info.participacion}</span>
            </div>
            <div class="index-box">
                <span class="index-title">Hipermedialidad</span>
                <span class="index-value">${node.info.hipermedialidad}</span>
            </div>
        `;
    } else { panel.style.display = 'none'; }
}

network.on("click", (p) => p.nodes.length > 0 ? showInfo(p.nodes[0]) : panel.style.display = 'none');
</script>

</body>
</html>



