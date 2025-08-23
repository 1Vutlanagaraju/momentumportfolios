export default function Homepage() {
  return (
    <div className="font-sans text-gray-900">
      {/* Header */}
      <header className="flex justify-between items-center px-8 py-4 shadow-md sticky top-0 bg-white z-50">
        <h1 className="text-2xl font-bold text-blue-900">MomentumPortfolios</h1>
        <nav className="hidden md:flex space-x-6">
          <a href="#" className="hover:text-green-600">Home</a>
          <a href="#" className="hover:text-green-600">About</a>
          <a href="#" className="hover:text-green-600">Services</a>
          <a href="#" className="hover:text-green-600">Performance</a>
          <a href="#" className="hover:text-green-600">Insights</a>
          <a href="#" className="hover:text-green-600">Contact</a>
        </nav>
        <button className="bg-green-600 text-white px-5 py-2 rounded-2xl shadow-md hover:bg-green-700">
          Start Investing
        </button>
      </header>

      {/* Hero Section */}
      <section className="bg-gradient-to-r from-blue-900 to-green-700 text-white text-center py-24 px-6">
        <h2 className="text-4xl font-bold mb-4">Accelerating Your Wealth with Smart Portfolios</h2>
        <p className="mb-6 text-lg">Data-driven portfolio strategies for long-term growth.</p>
        <div className="space-x-4">
          <button className="bg-white text-green-700 px-6 py-3 rounded-2xl font-semibold shadow-md">Get Started</button>
          <button className="border border-white px-6 py-3 rounded-2xl font-semibold">Book Free Consultation</button>
        </div>
      </section>

      {/* Why Momentum Section */}
      <section className="py-16 px-6 max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-4 gap-6 text-center">
        {[
          { icon: "📈", title: "Proven Returns", desc: "Beating benchmarks consistently" },
          { icon: "🔒", title: "Safe & Secure", desc: "SEBI-compliant & trusted" },
          { icon: "🧠", title: "Expert Research", desc: "Data-backed strategies" },
          { icon: "🤝", title: "Personalized Support", desc: "Tailored for every investor" }
        ].map((item, idx) => (
          <div key={idx} className="bg-white p-6 rounded-2xl shadow-md hover:shadow-lg">
            <div className="text-4xl mb-2">{item.icon}</div>
            <h3 className="font-bold text-lg mb-2">{item.title}</h3>
            <p className="text-gray-600 text-sm">{item.desc}</p>
          </div>
        ))}
      </section>

      {/* Services Section */}
      <section className="bg-gray-50 py-16 px-6">
        <h2 className="text-3xl font-bold text-center mb-12">Our Services</h2>
        <div className="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-4 gap-6">
          {[
            { title: "Portfolio Management", desc: "Tailored wealth solutions" },
            { title: "Stock Advisory", desc: "Actionable buy/sell calls" },
            { title: "Research Reports", desc: "Deep insights & analysis" },
            { title: "Wealth Planning", desc: "Long-term financial roadmap" }
          ].map((service, idx) => (
            <div key={idx} className="bg-white p-6 rounded-2xl shadow-md hover:shadow-lg text-center">
              <h3 className="font-bold text-lg mb-2">{service.title}</h3>
              <p className="text-gray-600 text-sm mb-3">{service.desc}</p>
              <button className="text-green-600 font-semibold">Learn More →</button>
            </div>
          ))}
        </div>
      </section>

      {/* Performance Snapshot */}
      <section className="py-16 px-6 text-center max-w-6xl mx-auto">
        <h2 className="text-3xl font-bold mb-6">Consistent Results. Proven Growth.</h2>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div className="bg-white p-6 rounded-2xl shadow-md">
            <h3 className="text-2xl font-bold text-green-600">+18% CAGR</h3>
            <p className="text-gray-600">Last 3 Years</p>
          </div>
          <div className="bg-white p-6 rounded-2xl shadow-md">
            <h3 className="text-2xl font-bold text-green-600">500+ Clients</h3>
            <p className="text-gray-600">Across India</p>
          </div>
          <div className="bg-white p-6 rounded-2xl shadow-md">
            <h3 className="text-2xl font-bold text-green-600">₹120 Cr+</h3>
            <p className="text-gray-600">Assets Managed</p>
          </div>
        </div>
      </section>

      {/* Testimonials */}
      <section className="bg-gray-50 py-16 px-6 text-center">
        <h2 className="text-3xl font-bold mb-10">What Our Clients Say</h2>
        <div className="max-w-4xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-6">
          <div className="bg-white p-6 rounded-2xl shadow-md">
            <p className="italic mb-3">“MomentumPortfolios helped me beat the market consistently.”</p>
            <h4 className="font-bold">– Investor A</h4>
          </div>
          <div className="bg-white p-6 rounded-2xl shadow-md">
