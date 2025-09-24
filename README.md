import React from 'react';
import { ShoppingCart, Users, TrendingUp, Clock, Home, Phone, MessageCircle, ChevronRight } from 'lucide-react';

const App = () => {
  const products = [
    {
      id: 1,
      name: "Aloe Vera Omnilife",
      description: "Bebida de aloe vera 100% pura para una digestión óptima y sistema inmunológico fortalecido.",
      regularPrice: 25.99,
      discountPrice: 20.79,
      image: "https://placehold.co/300x300/4ade80/ffffff?text=Aloe+Vera"
    },
    {
      id: 2,
      name: "Chiva Colágeno",
      description: "Colágeno hidrolizado con vitamina C para piel, cabello y articulaciones saludables.",
      regularPrice: 32.50,
      discountPrice: 26.00,
      image: "https://placehold.co/300x300/22c55e/ffffff?text=Chiva+Colágeno"
    },
    {
      id: 3,
      name: "Power Maker",
      description: "Suplemento energético natural con guaraná y ginseng para rendimiento físico y mental.",
      regularPrice: 68.50,
      discountPrice: 54.80,
      image: "https://placehold.co/300x300/16a34a/ffffff?text=Power+Maker"
    },
    {
      id: 4,
      name: "Angelíssima",
      description: "Fórmula exclusiva para el bienestar femenino con ingredientes naturales y vitaminas.",
      regularPrice: 35.00,
      discountPrice: 28.00,
      image: "https://placehold.co/300x300/15803d/ffffff?text=Angelíssima"
    }
  ];

  const testimonials = [
    {
      name: "María González",
      role: "Empresaria Omnilife desde 2021",
      text: "Gracias a Omnilife logré dejar mi trabajo de oficina y ahora viajo por el mundo mientras construyo mi negocio. Mis ingresos han triplicado en solo 18 meses.",
      image: "https://placehold.co/80x80/f1f5f9/64748b?text=MG"
    },
    {
      name: "Carlos Rodríguez",
      role: "Emprendedor desde 2022",
      text: "Empecé vendiendo a mis amigos y hoy tengo un equipo de 15 personas. La capacitación y el apoyo son increíbles. ¡Mi vida cambió por completo!",
      image: "https://placehold.co/80x80/f1f5f9/64748b?text=CR"
    },
    {
      name: "Ana Martínez",
      role: "Cliente y Empresaria",
      text: "Primero fui cliente por los productos de calidad, luego me afilié y ahora tengo ingresos residuales que me permiten estar más tiempo con mi familia.",
      image: "https://placehold.co/80x80/f1f5f9/64748b?text=AM"
    }
  ];

  const comparisonItems = [
    {
      traditional: "Ingresos fijos limitados",
      omnilife: "Ingresos escalables ilimitados"
    },
    {
      traditional: "Horario rígido de 8-5",
      omnilife: "Libertad de horarios y ubicación"
    },
    {
      traditional: "Crecimiento lento y limitado",
      omnilife: "Crecimiento exponencial con equipo"
    },
    {
      traditional: "Estrés constante y burnout",
      omnilife: "Equilibrio vida-trabajo y bienestar"
    },
    {
      traditional: "Dependencia de un solo empleador",
      omnilife: "Independencia financiera y múltiples fuentes de ingreso"
    }
  ];

  const whatsappLink = "https://wa.me/593999999999?text=Hola%20quiero%20más%20información%20sobre%20Omnilife";
  const registrationLink = "https://portal.omnilife.com/registro?distributor_code=593686430EAJ&country_code=ECU&lang=es";

  return (
    <div className="min-h-screen bg-white">
      {/* Header */}
      <header className="bg-white shadow-sm sticky top-0 z-50">
        <nav className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="flex justify-between items-center h-16">
            <div className="flex items-center">
              <div className="flex-shrink-0">
                <h1 className="text-2xl font-bold text-green-600">Omnilife</h1>
              </div>
            </div>
            <div className="hidden md:block">
              <div className="ml-10 flex items-baseline space-x-8">
                <a href="#inicio" className="text-gray-900 hover:text-green-600 px-3 py-2 text-sm font-medium">Inicio</a>
                <a href="#productos" className="text-gray-900 hover:text-green-600 px-3 py-2 text-sm font-medium">Productos</a>
                <a href="#oportunidad" className="text-gray-900 hover:text-green-600 px-3 py-2 text-sm font-medium">Oportunidad</a>
                <a href="#testimonios" className="text-gray-900 hover:text-green-600 px-3 py-2 text-sm font-medium">Testimonios</a>
                <a href="#afiliate" className="text-gray-900 hover:text-green-600 px-3 py-2 text-sm font-medium">Afíliate</a>
                <a href="#contacto" className="text-gray-900 hover:text-green-600 px-3 py-2 text-sm font-medium">Contacto</a>
              </div>
            </div>
          </div>
        </nav>
      </header>

      {/* Hero Section */}
      <section id="inicio" className="bg-gradient-to-br from-green-50 to-emerald-100 py-20">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center">
            <h1 className="text-4xl md:text-6xl font-bold text-gray-900 mb-6 leading-tight">
              Tu oportunidad de emprender con Omnilife:
              <span className="block text-green-600">producto de calidad + negocio escalable</span>
            </h1>
            <p className="text-xl text-gray-700 mb-8 max-w-4xl mx-auto">
              <span className="font-semibold">Compra como cliente con 20% de descuento</span> y disfruta de productos premium para tu salud. 
              <span className="font-semibold block mt-2">Afíliate con mi código</span> para ser empresario/emprendedor y construir ingresos residuales.
            </p>
            <div className="flex flex-col sm:flex-row gap-4 justify-center">
              <a 
                href={whatsappLink} 
                className="bg-green-600 hover:bg-green-700 text-white px-8 py-4 rounded-lg text-lg font-semibold transition-colors duration-300 flex items-center justify-center gap-2"
              >
                <ShoppingCart size={20} />
                Comprar ahora con descuento
              </a>
              <a 
                href={registrationLink} 
                className="bg-emerald-500 hover:bg-emerald-600 text-white px-8 py-4 rounded-lg text-lg font-semibold transition-colors duration-300 flex items-center justify-center gap-2"
              >
                <Users size={20} />
                Afíliarme como empresario
              </a>
            </div>
          </div>
        </div>
      </section>

      {/* Productos Section */}
      <section id="productos" className="py-20 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Productos Destacados</h2>
            <p className="text-xl text-gray-600">Descubre nuestra selección premium con 20% de descuento exclusivo</p>
          </div>
          
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
            {products.map((product) => (
              <div key={product.id} className="bg-white rounded-xl shadow-lg hover:shadow-xl transition-shadow duration-300 overflow-hidden">
                <img 
                  src={product.image} 
                  alt={product.name}
                  className="w-full h-48 object-cover"
                />
                <div className="p-6">
                  <h3 className="text-xl font-bold text-gray-900 mb-2">{product.name}</h3>
                  <p className="text-gray-600 mb-4">{product.description}</p>
                  <div className="flex items-center justify-between mb-4">
                    <span className="text-gray-500 line-through">${product.regularPrice}</span>
                    <span className="text-2xl font-bold text-green-600">${product.discountPrice}</span>
                  </div>
                  <a 
                    href={whatsappLink}
                    className="w-full bg-green-600 hover:bg-green-700 text-white py-3 rounded-lg font-semibold transition-colors duration-300 flex items-center justify-center gap-2"
                  >
                    <MessageCircle size={18} />
                    Comprar con descuento
                  </a>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Oportunidad de Negocio */}
      <section id="oportunidad" className="py-20 bg-gradient-to-br from-emerald-50 to-green-100">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Oportunidad de Negocio</h2>
            <p className="text-xl text-gray-600">Construye tu propio imperio con Omnilife</p>
          </div>
          
          <div className="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <div>
              <h3 className="text-2xl font-bold text-gray-900 mb-6">¿Qué significa ser empresario con Omnilife?</h3>
              <div className="space-y-4">
                <div className="flex items-start gap-3">
                  <TrendingUp className="text-green-600 mt-1 flex-shrink-0" size={24} />
                  <div>
                    <h4 className="font-semibold text-gray-900">Ingresos Residuales</h4>
                    <p className="text-gray-600">Gana comisiones continuas de tu red de distribuidores y clientes.</p>
                  </div>
                </div>
                <div className="flex items-start gap-3">
                  <Users className="text-green-600 mt-1 flex-shrink-0" size={24} />
                  <div>
                    <h4 className="font-semibold text-gray-900">Equipo de Apoyo</h4>
                    <p className="text-gray-600">Accede a capacitación constante y mentoría de líderes experimentados.</p>
                  </div>
                </div>
                <div className="flex items-start gap-3">
                  <Clock className="text-green-600 mt-1 flex-shrink-0" size={24} />
                  <div>
                    <h4 className="font-semibold text-gray-900">Libertad de Tiempo</h4>
                    <p className="text-gray-600">Trabaja desde cualquier lugar y en los horarios que elijas.</p>
                  </div>
                </div>
                <div className="flex items-start gap-3">
                  <Home className="text-green-600 mt-1 flex-shrink-0" size={24} />
                  <div>
                    <h4 className="font-semibold text-gray-900">Trabajo desde Casa</h4>
                    <p className="text-gray-600">Inicia tu negocio sin necesidad de oficina o inversión inicial grande.</p>
                  </div>
                </div>
              </div>
            </div>
            
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
              <div className="bg-white p-6 rounded-lg shadow-md">
                <img 
                  src="https://placehold.co/300x200/4ade80/ffffff?text=Emprendedor+1" 
                  alt="Emprendedor feliz"
                  className="w-full h-32 object-cover rounded-lg mb-4"
                />
                <p className="text-gray-700">Modelo de negocio probado con más de 30 años de éxito internacional.</p>
              </div>
              <div className="bg-white p-6 rounded-lg shadow-md">
                <img 
                  src="https://placehold.co/300x200/22c55e/ffffff?text=Equipo+Exitoso" 
                  alt="Equipo exitoso"
                  className="w-full h-32 object-cover rounded-lg mb-4"
                />
                <p className="text-gray-700">Escalabilidad ilimitada: tu esfuerzo se multiplica con cada persona que se une.</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Testimonios */}
      <section id="testimonios" className="py-20 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Historias de Éxito</h2>
            <p className="text-xl text-gray-600">Personas reales que transformaron sus vidas con Omnilife</p>
          </div>
          
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            {testimonials.map((testimonial, index) => (
              <div key={index} className="bg-gray-50 p-6 rounded-xl">
                <div className="flex items-center mb-4">
                  <img 
                    src={testimonial.image} 
                    alt={testimonial.name}
                    className="w-12 h-12 rounded-full mr-4"
                  />
                  <div>
                    <h4 className="font-bold text-gray-900">{testimonial.name}</h4>
                    <p className="text-sm text-gray-600">{testimonial.role}</p>
                  </div>
                </div>
                <p className="text-gray-700 italic">"{testimonial.text}"</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Comparativa */}
      <section className="py-20 bg-gradient-to-br from-green-50 to-emerald-100">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Trabajo Tradicional vs Omnilife</h2>
            <p className="text-xl text-gray-600">Elige tu camino hacia la libertad financiera</p>
          </div>
          
          <div className="bg-white rounded-2xl shadow-xl overflow-hidden">
            <div className="grid grid-cols-1 md:grid-cols-2">
              <div className="bg-red-50 p-8">
                <h3 className="text-2xl font-bold text-red-700 mb-6 text-center">Trabajo Tradicional</h3>
                <div className="space-y-4">
                  {comparisonItems.map((item, index) => (
                    <div key={index} className="border-l-4 border-red-500 pl-4 py-2">
                      <p className="text-gray-700">{item.traditional}</p>
                    </div>
                  ))}
                </div>
              </div>
              <div className="bg-green-50 p-8">
                <h3 className="text-2xl font-bold text-green-700 mb-6 text-center">Negocio Omnilife</h3>
                <div className="space-y-4">
                  {comparisonItems.map((item, index) => (
                    <div key={index} className="border-l-4 border-green-500 pl-4 py-2">
                      <p className="text-gray-700">{item.omnilife}</p>
                    </div>
                  ))}
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Cómo Afiliarse */}
      <section id="afiliate" className="py-20 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-3xl md:text-4xl font-bold text-gray-900 mb-4">¿Cómo Afiliarte?</h2>
            <p className="text-xl text-gray-600">Sigue estos simples pasos y comienza tu viaje</p>
          </div>
          
          <div className="max-w-4xl mx-auto">
            <div className="relative">
              <div className="absolute left-8 top-0 bottom-0 w-0.5 bg-green-200 transform -translate-x-1/2"></div>
              
              <div className="space-y-12 relative">
                {[1, 2, 3].map((step) => (
                  <div key={step} className="flex items-start">
                    <div className="flex-shrink-0 w-16 h-16 bg-green-600 rounded-full flex items-center justify-center text-white font-bold text-lg z-10">
                      {step}
                    </div>
                    <div className="ml-8 flex-1">
                      {step === 1 && (
                        <>
                          <h3 className="text-xl font-bold text-gray-900 mb-2">Contáctame por WhatsApp</h3>
                          <p className="text-gray-600">Escríbeme para resolver todas tus dudas y guiarte en el proceso.</p>
                        </>
                      )}
                      {step === 2 && (
                        <>
                          <h3 className="text-xl font-bold text-gray-900 mb-2">Completa tu afiliación</h3>
                          <p className="text-gray-600">
                            Usa mi código exclusivo: <a href={registrationLink} className="text-green-600 hover:underline font-semibold">593686430EAJ</a>
                          </p>
                        </>
                      )}
                      {step === 3 && (
                        <>
                          <h3 className="text-xl font-bold text-gray-900 mb-2">Accede a beneficios y capacitación</h3>
                          <p className="text-gray-600">Recibe formación continua, materiales de marketing y comienza a vender e invitar.</p>
                        </>
                      )}
                    </div>
                  </div>
                ))}
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* CTA Final */}
      <section id="contacto" className="py-20 bg-gradient-to-r from-green-600 to-emerald-700">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
          <h2 className="text-3xl md:text-4xl font-bold text-white mb-6">
            Elige tu camino hacia el éxito
          </h2>
          <p className="text-xl text-green-100 mb-8 max-w-3xl mx-auto">
            <span className="block mb-2">Compra ahora con -20% como cliente</span>
            <span className="block">o</span>
            <span className="block mt-2">Únete conmigo como empresario y cambia tu vida</span>
          </p>
          
          <div className="flex flex-col sm:flex-row gap-6 justify-center mb-8">
            <a 
              href={whatsappLink}
              className="bg-white text-green-600 hover:bg-green-50 px-8 py-4 rounded-lg text-lg font-semibold transition-colors duration-300 flex items-center justify-center gap-2"
            >
              <Phone size={20} />
              WhatsApp: +593 99 572 0816
            </a>
            <a 
              href={registrationLink}
              className="bg-emerald-500 hover:bg-emerald-600 text-white px-8 py-4 rounded-lg text-lg font-semibold transition-colors duration-300 flex items-center justify-center gap-2"
            >
              <Users size={20} />
              Afíliate Ahora
            </a>
          </div>
          
          <div className="bg-white/10 backdrop-blur-sm rounded-lg p-6 max-w-2xl mx-auto">
            <h3 className="text-xl font-bold text-white mb-4">¿Tienes preguntas?</h3>
            <p className="text-green-100">
              No dudes en contactarme. Estoy aquí para ayudarte a tomar la mejor decisión para tu futuro.
            </p>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-gray-900 text-white py-8">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
          <p className="text-gray-400">
            © 2024 Omnilife - Distribuidor Independiente | Código: 593686430EAJ
          </p>
          <p className="text-gray-500 text-sm mt-2">
            Productos de alta calidad para tu salud y bienestar
          </p>
        </div>
      </footer>
    </div>
  );
};

export default App;
