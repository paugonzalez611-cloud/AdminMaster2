import React, { useState, useEffect, useRef } from 'react';
import {
  MessageSquare, Target, BarChart3, Palette, Users,
  ArrowRight, ChevronLeft, Search, BookOpen, Zap, TrendingUp, Award
} from 'lucide-react';

const FONTS = `@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,700;0,9..144,900;1,9..144,400&family=Syne:wght@400;600;700;800&display=swap');`;

const CHATBOTS = [
  {
    id: 'community-manager',
    name: 'Elena Social',
    role: 'Community Manager',
    icon: <Users className="w-5 h-5" />,
    accent: '#3B82F6',
    accentLight: '#EFF6FF',
    accentDark: '#1D4ED8',
    tag: 'Redes & Comunidad',
    description: 'Experta en gestión de comunidades y tono de voz en redes sociales.',
    personality: 'Cercana, energética y siempre al día con las tendencias.',
    chat: [
      { role: 'user', content: '¿Cómo podemos mejorar el engagement en nuestra nueva campaña de lanzamiento?' },
      { role: 'bot', content: '¡Hola! Para el lanzamiento, no solo publiquemos anuncios. Necesitamos Storytelling. Sugiero crear una serie de "detrás de escena" en Stories y un concurso interactivo que premie la lealtad. Recuerda: la CIM exige que el tono en Instagram sea el mismo que en tu sitio web, pero adaptado a la calidez de la red.' },
      { role: 'user', content: '¿Qué hacemos si recibimos críticas negativas en los comentarios?' },
      { role: 'bot', content: 'La transparencia es clave en CIM. Responde rápido, con empatía y siempre alineado a los valores de la marca. Una respuesta coherente transforma un problema en una oportunidad de servicio al cliente.' }
    ]
  },
  {
    id: 'estratega',
    name: 'Marcus Plan',
    role: 'Estratega CIM',
    icon: <Target className="w-5 h-5" />,
    accent: '#6366F1',
    accentLight: '#EEF2FF',
    accentDark: '#4338CA',
    tag: 'Estrategia Global',
    description: 'Especialista en alineación estratégica y omnicanalidad.',
    personality: 'Profesional, estructurado y enfocado en la visión global.',
    chat: [
      { role: 'user', content: '¿Cómo aseguramos que el mensaje sea coherente en todos los canales?' },
      { role: 'bot', content: 'La clave es el "Manual de Identidad de Campaña". Antes de ejecutar, definimos un mensaje central único. Si en TV decimos "Innovación para todos", en el mailing no podemos enfocarnos solo en "Precio bajo". La omnicanalidad significa que el cliente siente la misma marca, sin importar dónde nos encuentre.' },
      { role: 'user', content: '¿Cuál es el error más común al intentar integrar canales?' },
      { role: 'bot', content: 'Trabajar en silos. El equipo de redes no habla con el de ventas. La CIM rompe esas barreras para que la experiencia del usuario sea fluida y sin contradicciones.' }
    ]
  },
  {
    id: 'analista',
    name: 'Dr. Data',
    role: 'Analista de Métricas',
    icon: <BarChart3 className="w-5 h-5" />,
    accent: '#F97316',
    accentLight: '#FFF7ED',
    accentDark: '#C2410C',
    tag: 'ROI & Analytics',
    description: 'Experto en ROI, conversión y comportamiento del consumidor.',
    personality: 'Preciso, lógico y basado en evidencias numéricas.',
    chat: [
      { role: 'user', content: '¿Qué KPIs son los más importantes para medir el éxito de una estrategia CIM?' },
      { role: 'bot', content: 'No te pierdas en las métricas de vanidad. Para CIM, analizamos el Atribución Multi-Touch. Debemos mirar el CTR, la Tasa de Conversión Cruzada y, sobre todo, el Valor de Vida del Cliente (CLV). El éxito no es una venta aislada, es la sinergia de los puntos de contacto.' },
      { role: 'user', content: '¿Cómo sabemos si la integración de canales está funcionando?' },
      { role: 'bot', content: 'Si el costo de adquisición (CAC) baja mientras la recordación de marca sube, la integración es efectiva. Los datos no mienten: la coherencia genera confianza, y la confianza genera ventas.' }
    ]
  },
  {
    id: 'creativo',
    name: 'Santi Creativo',
    role: 'Creativo Publicitario',
    icon: <Palette className="w-5 h-5" />,
    accent: '#A855F7',
    accentLight: '#FAF5FF',
    accentDark: '#7E22CE',
    tag: 'Creatividad Visual',
    description: 'Especialista en conceptos visuales e impacto emocional.',
    personality: 'Inspirador, visual y disruptivo.',
    chat: [
      { role: 'user', content: '¿Cómo crear una campaña visualmente impactante que respete la CIM?' },
      { role: 'bot', content: '¡La magia está en la consistencia! No se trata de repetir la misma imagen, sino de usar una "constante visual" (colores, tipografía, estilo fotográfico). Si el usuario ve un post y luego un cartel en la calle, debe reconocer la marca en 2 segundos, incluso sin ver el logo.' },
      { role: 'user', content: '¿Es más importante la creatividad o el mensaje?' },
      { role: 'bot', content: 'En CIM son inseparables. Una creatividad brillante sin un mensaje coherente es solo ruido. Diseñamos para emocionar, pero siempre bajo el paraguas de la estrategia de comunicación.' }
    ]
  }
];

const PILLARS = [
  { num: '01', title: 'Coherencia', desc: 'Los mensajes deben relacionarse entre sí y reforzar un mensaje central único a través de todos los puntos de contacto.', color: '#3B82F6' },
  { num: '02', title: 'Consistencia', desc: 'El mensaje no puede ser contradictorio. La marca debe hablar con una sola voz sin importar el canal.', color: '#6366F1' },
  { num: '03', title: 'Continuidad', desc: 'Comunicación sostenida en el tiempo que construye reconocimiento y confianza de forma progresiva.', color: '#F97316' },
  { num: '04', title: 'Complementariedad', desc: 'La suma de las partes es mayor al todo. Cada canal amplifica el impacto de los demás.', color: '#A855F7' },
];

const globalStyles = `
  ${FONTS}
  .cim-display { font-family: 'Fraunces', serif; }
  .cim-ui { font-family: 'Syne', sans-serif; }
  .cim-body { font-family: 'Syne', sans-serif; }
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }
  @keyframes shimmer {
    0% { background-position: -200% center; }
    100% { background-position: 200% center; }
  }
  .fade-up { animation: fadeUp 0.6s cubic-bezier(0.16,1,0.3,1) both; }
  .fade-up-1 { animation-delay: 0.05s; }
  .fade-up-2 { animation-delay: 0.12s; }
  .fade-up-3 { animation-delay: 0.2s; }
  .fade-up-4 { animation-delay: 0.28s; }
  .shimmer-text {
    background: linear-gradient(90deg, #1e3a8a 0%, #3b82f6 30%, #818cf8 50%, #3b82f6 70%, #1e3a8a 100%);
    background-size: 200% auto;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: shimmer 4s linear infinite;
  }
  .bot-card:hover .bot-card-inner { transform: translateY(-4px); box-shadow: 0 24px 48px -12px rgba(0,0,0,0.12); }
  .bot-card-inner { transition: transform 0.3s cubic-bezier(0.16,1,0.3,1), box-shadow 0.3s ease; }
  .nav-link { position: relative; }
  .nav-link::after { content: ''; position: absolute; bottom: -2px; left: 0; width: 0; height: 2px; background: #3b82f6; transition: width 0.2s ease; }
  .nav-link.active::after, .nav-link:hover::after { width: 100%; }
  .chat-bubble-bot { animation: fadeUp 0.3s ease both; }
  .pillar-card:hover { border-color: var(--pillar-color) !important; }
  .pillar-card { transition: border-color 0.2s ease, transform 0.2s ease; }
  .pillar-card:hover { transform: translateY(-2px); }
  .hero-bg {
    background: radial-gradient(ellipse 80% 60% at 50% -10%, rgba(59,130,246,0.08) 0%, transparent 70%),
                radial-gradient(ellipse 40% 40% at 90% 80%, rgba(99,102,241,0.06) 0%, transparent 60%),
                #FAFAFA;
  }
  .stat-pill {
    display: inline-flex; align-items: center; gap: 6px;
    background: white; border: 1px solid #E5E7EB;
    border-radius: 100px; padding: 6px 14px;
    font-size: 13px; color: #374151; font-weight: 600;
    box-shadow: 0 1px 3px rgba(0,0,0,0.06);
  }
`;

export default function App() {
  const [view, setView] = useState('landing');
  const [selectedBot, setSelectedBot] = useState(null);
  const [searchQuery, setSearchQuery] = useState('');
  const chatEndRef = useRef(null);

  useEffect(() => {
    if (view === 'chat' && chatEndRef.current) {
      chatEndRef.current.scrollIntoView({ behavior: 'smooth' });
    }
  }, [view]);

  const filteredBots = CHATBOTS.filter(bot =>
    bot.name.toLowerCase().includes(searchQuery.toLowerCase()) ||
    bot.role.toLowerCase().includes(searchQuery.toLowerCase())
  );

  const navigate = (dest) => {
    setView(dest);
  };

  const renderLanding = () => (
    <div className="hero-bg min-h-screen">
      <div className="max-w-5xl mx-auto px-6 pt-24 pb-20 text-center">
        <div className="fade-up fade-up-1 mb-5 inline-flex items-center gap-2 stat-pill">
          <span style={{ width: 8, height: 8, borderRadius: '50%', background: '#22C55E', display: 'inline-block' }} />
          Simulador Interactivo · 4 Expertos Virtuales
        </div>

        <h1 className="cim-display fade-up fade-up-2 mb-6"
          style={{ fontSize: 'clamp(52px, 8vw, 88px)', fontWeight: 900, lineHeight: 1.0, letterSpacing: '-2px', color: '#0F172A' }}>
          Domina la<br />
          <span className="shimmer-text">Comunicación</span><br />
          <span style={{ fontStyle: 'italic', fontWeight: 300 }}>Integrada</span>
        </h1>

        <p className="cim-body fade-up fade-up-3 mx-auto mb-10"
          style={{ fontSize: 18, lineHeight: 1.7, color: '#64748B', maxWidth: 520 }}>
          Aprende CIM a través de conversaciones reales con expertos virtuales especializados en cada área del marketing integrado.
        </p>

        <div className="fade-up fade-up-4 flex flex-col sm:flex-row gap-3 justify-center mb-20">
          <button onClick={() => navigate('dashboard')}
            className="cim-ui"
            style={{
              display: 'inline-flex', alignItems: 'center', gap: 10,
              background: '#0F172A', color: 'white', border: 'none',
              borderRadius: 14, padding: '16px 32px', fontSize: 15, fontWeight: 700,
              cursor: 'pointer', transition: 'all 0.2s ease',
              boxShadow: '0 4px 14px rgba(15,23,42,0.2)'
            }}
            onMouseEnter={e => e.currentTarget.style.background = '#1E293B'}
            onMouseLeave={e => e.currentTarget.style.background = '#0F172A'}
          >
            Explorar Expertos <ArrowRight size={18} />
          </button>
          <button onClick={() => navigate('education')}
            className="cim-ui"
            style={{
              display: 'inline-flex', alignItems: 'center', gap: 10,
              background: 'white', color: '#374151', border: '1.5px solid #E5E7EB',
              borderRadius: 14, padding: '16px 32px', fontSize: 15, fontWeight: 700,
              cursor: 'pointer', transition: 'all 0.2s ease'
            }}
            onMouseEnter={e => { e.currentTarget.style.borderColor = '#3B82F6'; e.currentTarget.style.color = '#3B82F6'; }}
            onMouseLeave={e => { e.currentTarget.style.borderColor = '#E5E7EB'; e.currentTarget.style.color = '#374151'; }}
          >
            <BookOpen size={18} /> ¿Qué es la CIM?
          </button>
        </div>

        {/* Expert Preview Cards */}
        <div className="grid grid-cols-2 md:grid-cols-4 gap-3 fade-up" style={{ animationDelay: '0.35s' }}>
          {CHATBOTS.map((bot, i) => (
            <div key={bot.id} onClick={() => { setSelectedBot(bot); navigate('chat'); }}
              style={{
                background: 'white', borderRadius: 16, padding: '20px 16px', textAlign: 'left',
                border: '1px solid #F1F5F9', cursor: 'pointer', transition: 'all 0.25s ease',
                boxShadow: '0 1px 4px rgba(0,0,0,0.05)'
              }}
              onMouseEnter={e => { e.currentTarget.style.borderColor = bot.accent; e.currentTarget.style.transform = 'translateY(-3px)'; e.currentTarget.style.boxShadow = `0 8px 24px rgba(0,0,0,0.1)`; }}
              onMouseLeave={e => { e.currentTarget.style.borderColor = '#F1F5F9'; e.currentTarget.style.transform = 'translateY(0)'; e.currentTarget.style.boxShadow = '0 1px 4px rgba(0,0,0,0.05)'; }}
            >
              <div style={{ width: 36, height: 36, borderRadius: 10, background: bot.accentLight, display: 'flex', alignItems: 'center', justifyContent: 'center', color: bot.accent, marginBottom: 10 }}>
                {bot.icon}
              </div>
              <p className="cim-ui" style={{ fontSize: 13, fontWeight: 700, color: '#0F172A', marginBottom: 2 }}>{bot.name}</p>
              <p className="cim-ui" style={{ fontSize: 11, color: bot.accent, fontWeight: 600 }}>{bot.tag}</p>
            </div>
          ))}
        </div>
      </div>
    </div>
  );

  const renderDashboard = () => (
    <div className="max-w-6xl mx-auto px-6 py-14">
      <div className="flex flex-col md:flex-row md:items-end justify-between mb-12 gap-6">
        <div className="fade-up">
          <p className="cim-ui mb-2" style={{ fontSize: 12, fontWeight: 700, letterSpacing: '0.12em', color: '#94A3B8', textTransform: 'uppercase' }}>Panel de Expertos</p>
          <h2 className="cim-display" style={{ fontSize: 44, fontWeight: 900, color: '#0F172A', lineHeight: 1.1, letterSpacing: '-1px' }}>
            Elige tu<br /><span style={{ fontStyle: 'italic', fontWeight: 300 }}>especialista</span>
          </h2>
        </div>
        <div className="fade-up fade-up-2" style={{ position: 'relative', flexShrink: 0 }}>
          <Search style={{ position: 'absolute', left: 14, top: '50%', transform: 'translateY(-50%)', color: '#94A3B8', width: 16, height: 16 }} />
          <input
            type="text"
            placeholder="Buscar experto..."
            className="cim-ui"
            style={{
              paddingLeft: 40, paddingRight: 16, paddingTop: 11, paddingBottom: 11,
              border: '1.5px solid #E5E7EB', borderRadius: 12, width: 240,
              fontSize: 14, color: '#374151', background: 'white', outline: 'none',
              transition: 'border-color 0.2s'
            }}
            value={searchQuery}
            onChange={e => setSearchQuery(e.target.value)}
            onFocus={e => e.target.style.borderColor = '#3B82F6'}
            onBlur={e => e.target.style.borderColor = '#E5E7EB'}
          />
        </div>
      </div>

      <div className="grid grid-cols-1 md:grid-cols-2 gap-5">
        {filteredBots.map((bot, i) => (
          <div key={bot.id} className="bot-card fade-up"
            style={{ animationDelay: `${i * 0.08}s`, cursor: 'pointer' }}
            onClick={() => { setSelectedBot(bot); navigate('chat'); }}>
            <div className="bot-card-inner"
              style={{ background: 'white', borderRadius: 20, border: '1px solid #F1F5F9', overflow: 'hidden' }}>
              {/* Card header bar */}
              <div style={{ height: 5, background: `linear-gradient(90deg, ${bot.accent}, ${bot.accentDark})` }} />
              <div style={{ padding: '24px 28px' }}>
                <div style={{ display: 'flex', alignItems: 'flex-start', justifyContent: 'space-between', marginBottom: 16 }}>
                  <div style={{ display: 'flex', alignItems: 'center', gap: 14 }}>
                    <div style={{ width: 48, height: 48, borderRadius: 14, background: bot.accentLight, display: 'flex', alignItems: 'center', justifyContent: 'center', color: bot.accent, flexShrink: 0 }}>
                      {React.cloneElement(bot.icon, { size: 22 })}
                    </div>
                    <div>
                      <h3 className="cim-ui" style={{ fontSize: 18, fontWeight: 800, color: '#0F172A', marginBottom: 2 }}>{bot.name}</h3>
                      <span className="cim-ui" style={{ fontSize: 12, fontWeight: 700, color: bot.accent, background: bot.accentLight, padding: '3px 10px', borderRadius: 100 }}>{bot.tag}</span>
                    </div>
                  </div>
                  <div style={{ width: 32, height: 32, borderRadius: 10, border: '1.5px solid #E5E7EB', display: 'flex', alignItems: 'center', justifyContent: 'center', color: '#94A3B8', flexShrink: 0 }}>
                    <ArrowRight size={15} />
                  </div>
                </div>

                <p className="cim-body" style={{ fontSize: 14, color: '#64748B', lineHeight: 1.6, marginBottom: 16 }}>{bot.description}</p>

                <div style={{ borderTop: '1px solid #F8FAFC', paddingTop: 14, display: 'flex', alignItems: 'center', justifyContent: 'space-between' }}>
                  <p className="cim-ui" style={{ fontSize: 12, color: '#94A3B8', fontStyle: 'italic' }}>"{bot.personality}"</p>
                  <div style={{ display: 'flex', gap: 4 }}>
                    {bot.chat.filter(m => m.role === 'user').map((_, j) => (
                      <div key={j} style={{ width: 6, height: 6, borderRadius: '50%', background: bot.accentLight, border: `1.5px solid ${bot.accent}` }} />
                    ))}
                  </div>
                </div>
              </div>
            </div>
          </div>
        ))}
      </div>
    </div>
  );

  const renderChat = () => (
    <div className="max-w-3xl mx-auto px-4 py-8">
      <button onClick={() => navigate('dashboard')}
        className="cim-ui fade-up"
        style={{ display: 'inline-flex', alignItems: 'center', gap: 6, color: '#64748B', background: 'none', border: 'none', cursor: 'pointer', fontSize: 14, fontWeight: 600, marginBottom: 24, padding: 0 }}
        onMouseEnter={e => e.currentTarget.style.color = '#3B82F6'}
        onMouseLeave={e => e.currentTarget.style.color = '#64748B'}
      >
        <ChevronLeft size={18} /> Volver al panel
      </button>

      <div className="fade-up fade-up-1" style={{ background: 'white', borderRadius: 24, overflow: 'hidden', border: '1px solid #F1F5F9', boxShadow: '0 20px 60px rgba(0,0,0,0.08)', display: 'flex', flexDirection: 'column', minHeight: '72vh' }}>
        {/* Header */}
        <div style={{ background: `linear-gradient(135deg, ${selectedBot.accentDark} 0%, ${selectedBot.accent} 100%)`, padding: '24px 28px' }}>
          <div style={{ display: 'flex', alignItems: 'center', gap: 16 }}>
            <div style={{ width: 52, height: 52, borderRadius: 16, background: 'rgba(255,255,255,0.15)', display: 'flex', alignItems: 'center', justifyContent: 'center', color: 'white', backdropFilter: 'blur(4px)' }}>
              {React.cloneElement(selectedBot.icon, { size: 22 })}
            </div>
            <div>
              <h3 className="cim-ui" style={{ fontSize: 20, fontWeight: 800, color: 'white', marginBottom: 2 }}>{selectedBot.name}</h3>
              <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
                <span style={{ width: 8, height: 8, borderRadius: '50%', background: '#4ADE80', display: 'inline-block' }} />
                <span className="cim-ui" style={{ fontSize: 13, color: 'rgba(255,255,255,0.75)', fontWeight: 600 }}>{selectedBot.role} · Caso Práctico</span>
              </div>
            </div>
          </div>
        </div>

        {/* Personality */}
        <div style={{ background: '#FAFAFA', padding: '10px 28px', borderBottom: '1px solid #F1F5F9', display: 'flex', alignItems: 'center', gap: 8 }}>
          <Zap size={13} style={{ color: selectedBot.accent }} />
          <p className="cim-body" style={{ fontSize: 12, color: '#94A3B8', fontStyle: 'italic' }}>Personalidad: {selectedBot.personality}</p>
        </div>

        {/* Messages */}
        <div style={{ flex: 1, overflowY: 'auto', padding: '28px', display: 'flex', flexDirection: 'column', gap: 20, background: '#FDFCFF' }}>
          {selectedBot.chat.map((msg, idx) => (
            <div key={idx} style={{ display: 'flex', justifyContent: msg.role === 'user' ? 'flex-end' : 'flex-start' }}>
              {msg.role === 'bot' && (
                <div style={{ width: 32, height: 32, borderRadius: 10, background: selectedBot.accentLight, display: 'flex', alignItems: 'center', justifyContent: 'center', color: selectedBot.accent, flexShrink: 0, marginRight: 10, alignSelf: 'flex-end' }}>
                  {React.cloneElement(selectedBot.icon, { size: 14 })}
                </div>
              )}
              <div className={msg.role === 'bot' ? 'chat-bubble-bot' : ''}
                style={{
                  maxWidth: '78%', padding: '14px 18px', borderRadius: msg.role === 'user' ? '18px 18px 4px 18px' : '18px 18px 18px 4px',
                  background: msg.role === 'user' ? `linear-gradient(135deg, ${selectedBot.accentDark}, ${selectedBot.accent})` : 'white',
                  color: msg.role === 'user' ? 'white' : '#1E293B',
                  border: msg.role === 'bot' ? '1px solid #F1F5F9' : 'none',
                  boxShadow: msg.role === 'bot' ? '0 2px 8px rgba(0,0,0,0.06)' : '0 4px 12px rgba(0,0,0,0.15)',
                  animationDelay: `${idx * 0.15}s`
                }}>
                <p className="cim-body" style={{ fontSize: 14, lineHeight: 1.65 }}>{msg.content}</p>
              </div>
            </div>
          ))}
          <div ref={chatEndRef} />
        </div>

        {/* Input placeholder */}
        <div style={{ padding: '16px 20px', background: 'white', borderTop: '1px solid #F1F5F9' }}>
          <div className="cim-body" style={{ display: 'flex', alignItems: 'center', gap: 10, background: '#F8FAFC', borderRadius: 50, padding: '12px 20px', color: '#94A3B8', fontSize: 14 }}>
            <MessageSquare size={15} />
            Conversación de ejemplo · Solo lectura
          </div>
        </div>
      </div>
    </div>
  );

  const renderEducation = () => (
    <div className="max-w-4xl mx-auto px-6 py-12">
      <button onClick={() => navigate('landing')}
        className="cim-ui fade-up"
        style={{ display: 'inline-flex', alignItems: 'center', gap: 6, color: '#64748B', background: 'none', border: 'none', cursor: 'pointer', fontSize: 14, fontWeight: 600, marginBottom: 32, padding: 0 }}
        onMouseEnter={e => e.currentTarget.style.color = '#3B82F6'}
        onMouseLeave={e => e.currentTarget.style.color = '#64748B'}
      >
        <ChevronLeft size={18} /> Volver al inicio
      </button>

      <div className="fade-up fade-up-1 mb-14">
        <p className="cim-ui mb-3" style={{ fontSize: 12, fontWeight: 700, letterSpacing: '0.12em', color: '#94A3B8', textTransform: 'uppercase' }}>Marco Teórico</p>
        <h2 className="cim-display mb-5" style={{ fontSize: 52, fontWeight: 900, color: '#0F172A', lineHeight: 1.05, letterSpacing: '-1.5px' }}>
          ¿Qué es la<br /><span style={{ fontStyle: 'italic', fontWeight: 300 }}>CIM?</span>
        </h2>
        <p className="cim-body" style={{ fontSize: 17, lineHeight: 1.75, color: '#64748B', maxWidth: 600, borderLeft: '3px solid #3B82F6', paddingLeft: 20 }}>
          La Comunicación Integrada de Marketing es el proceso de coordinar y unificar todos los canales de una empresa para ofrecer un mensaje claro, coherente y continuo al consumidor.
        </p>
      </div>

      {/* Pillars */}
      <div className="mb-14">
        <h3 className="cim-ui mb-6" style={{ fontSize: 13, fontWeight: 700, color: '#94A3B8', letterSpacing: '0.1em', textTransform: 'uppercase' }}>Los 4 Pilares</h3>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
          {PILLARS.map((p, i) => (
            <div key={i} className="pillar-card fade-up"
              style={{
                '--pillar-color': p.color,
                animationDelay: `${i * 0.08}s`,
                background: 'white', border: '1.5px solid #F1F5F9', borderRadius: 18,
                padding: '24px 26px', display: 'flex', gap: 18
              }}>
              <span className="cim-display" style={{ fontSize: 48, fontWeight: 900, color: '#F1F5F9', lineHeight: 1, flexShrink: 0 }}>{p.num}</span>
              <div>
                <h4 className="cim-ui" style={{ fontSize: 17, fontWeight: 800, color: p.color, marginBottom: 6 }}>{p.title}</h4>
                <p className="cim-body" style={{ fontSize: 14, color: '#64748B', lineHeight: 1.6 }}>{p.desc}</p>
              </div>
            </div>
          ))}
        </div>
      </div>

      {/* Benefits */}
      <div className="fade-up fade-up-3 mb-12"
        style={{ background: '#FAFAFA', borderRadius: 20, border: '1px solid #F1F5F9', padding: '32px 36px' }}>
        <h3 className="cim-ui mb-6" style={{ fontSize: 13, fontWeight: 700, color: '#94A3B8', letterSpacing: '0.1em', textTransform: 'uppercase' }}>Beneficios clave</h3>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
          {[
            { icon: <TrendingUp size={18} />, label: 'Mayor recordación de marca', color: '#3B82F6' },
            { icon: <Award size={18} />, label: 'Confianza del consumidor', color: '#6366F1' },
            { icon: <Zap size={18} />, label: 'Experiencia de usuario unificada', color: '#F97316' },
            { icon: <BarChart3 size={18} />, label: 'Ahorro en costos de producción', color: '#A855F7' },
          ].map((b, i) => (
            <div key={i} style={{ display: 'flex', alignItems: 'center', gap: 12, background: 'white', borderRadius: 12, padding: '14px 18px', border: '1px solid #F1F5F9' }}>
              <div style={{ color: b.color, flexShrink: 0 }}>{b.icon}</div>
              <p className="cim-ui" style={{ fontSize: 14, fontWeight: 600, color: '#374151' }}>{b.label}</p>
            </div>
          ))}
        </div>
      </div>

      {/* CTA */}
      <div className="fade-up fade-up-4 text-center"
        style={{ background: 'linear-gradient(135deg, #0F172A 0%, #1E3A8A 100%)', borderRadius: 24, padding: '52px 40px' }}>
        <h3 className="cim-display mb-3" style={{ fontSize: 38, fontWeight: 900, color: 'white', lineHeight: 1.1 }}>
          ¿Listo para<br /><span style={{ fontStyle: 'italic', fontWeight: 300 }}>practicar?</span>
        </h3>
        <p className="cim-body mb-8" style={{ fontSize: 15, color: 'rgba(255,255,255,0.55)', lineHeight: 1.6 }}>
          Aplica estos conceptos en conversaciones reales con nuestros expertos virtuales.
        </p>
        <button onClick={() => navigate('dashboard')}
          className="cim-ui"
          style={{
            background: 'white', color: '#0F172A', border: 'none', borderRadius: 14,
            padding: '16px 36px', fontSize: 15, fontWeight: 800, cursor: 'pointer',
            transition: 'all 0.2s ease'
          }}
          onMouseEnter={e => e.currentTarget.style.transform = 'translateY(-2px)'}
          onMouseLeave={e => e.currentTarget.style.transform = 'translateY(0)'}
        >
          Hablar con los Expertos →
        </button>
      </div>
    </div>
  );

  return (
    <div style={{ minHeight: '100vh', background: '#FAFAFA', fontFamily: 'Syne, sans-serif' }}>
      <style>{globalStyles}</style>

      {/* Navbar */}
      <nav style={{
        position: 'sticky', top: 0, zIndex: 50,
        background: 'rgba(250,250,250,0.85)', backdropFilter: 'blur(16px)',
        borderBottom: '1px solid rgba(0,0,0,0.06)', padding: '0 24px'
      }}>
        <div style={{ maxWidth: 1152, margin: '0 auto', display: 'flex', alignItems: 'center', justifyContent: 'space-between', height: 64 }}>
          <div onClick={() => navigate('landing')}
            style={{ display: 'flex', alignItems: 'center', gap: 10, cursor: 'pointer' }}>
            <div style={{ width: 36, height: 36, background: '#0F172A', borderRadius: 10, display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
              <Target size={18} color="white" />
            </div>
            <span className="cim-ui" style={{ fontSize: 18, fontWeight: 800, color: '#0F172A', letterSpacing: '-0.5px' }}>Admin Master</span>
          </div>

          <div style={{ display: 'flex', alignItems: 'center', gap: 32 }}>
            {[
              { label: 'Inicio', dest: 'landing' },
              { label: 'Expertos', dest: 'dashboard' },
              { label: 'Conceptos', dest: 'education' },
            ].map(link => (
              <button key={link.dest} onClick={() => navigate(link.dest)}
                className={`nav-link cim-ui ${view === link.dest || (link.dest === 'dashboard' && view === 'chat') ? 'active' : ''}`}
                style={{ background: 'none', border: 'none', cursor: 'pointer', fontSize: 14, fontWeight: 700, color: view === link.dest || (link.dest === 'dashboard' && view === 'chat') ? '#0F172A' : '#94A3B8', padding: '4px 0' }}>
                {link.label}
              </button>
            ))}
          </div>

          <button onClick={() => navigate('dashboard')}
            className="cim-ui"
            style={{
              background: '#3B82F6', color: 'white', border: 'none', borderRadius: 100,
              padding: '10px 22px', fontSize: 13, fontWeight: 700, cursor: 'pointer',
              transition: 'all 0.2s ease', boxShadow: '0 2px 8px rgba(59,130,246,0.3)'
            }}
            onMouseEnter={e => e.currentTarget.style.background = '#2563EB'}
            onMouseLeave={e => e.currentTarget.style.background = '#3B82F6'}
          >
            Empezar →
          </button>
        </div>
      </nav>

      {/* Content */}
      <main>
        {view === 'landing' && renderLanding()}
        {view === 'dashboard' && renderDashboard()}
        {view === 'chat' && selectedBot && renderChat()}
        {view === 'education' && renderEducation()}
      </main>

      {/* Footer */}
      <footer style={{ marginTop: 80, borderTop: '1px solid #F1F5F9', padding: '36px 24px', textAlign: 'center' }}>
        <p className="cim-ui" style={{ fontSize: 13, color: '#CBD5E1' }}>© 2025 Admin Master · Simulador de Marketing Interactivo</p>
      </footer>
    </div>
  );
}
