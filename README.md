export default function ChurchMinistryWebsite() {
  const services = [
    {
      title: 'Sunday Worship',
      time: 'Sundays • 10:00 AM',
      description: 'A welcoming worship experience with prayer, music, and a message of hope.',
    },
    {
      title: 'Bible Study',
      time: 'Wednesdays • 7:00 PM',
      description: 'Grow deeper in faith through scripture study and meaningful discussion.',
    },
    {
      title: 'Community Outreach',
      time: 'Monthly Events',
      description: 'Serving families, youth, and individuals through local outreach and support.',
    },
  ];

  const ministries = [
    'Youth Ministry',
    'Prayer Team',
    'Women’s Fellowship',
    'Men’s Fellowship',
    'Children’s Ministry',
    'Community Service',
  ];

  return (
    <div className="min-h-screen bg-gradient-to-br from-slate-950 via-blue-950 through-indigo-950 to-sky-900 text-white">
      {/* Hero Section */}
      <section className="relative overflow-hidden before:absolute before:inset-0 before:bg-[radial-gradient(circle_at_center,rgba(255,255,255,0.15),transparent_60%)] bg-[radial-gradient(circle_at_top_left,#60a5fa_0%,#2563eb_25%,#1e3a8a_55%,#020617_100%)] text-white">
        <div className="absolute inset-0 opacity-30 bg-[radial-gradient(circle_at_top_right,white,transparent_35%)]" />
        <div className="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1504052434569-70ad5836ab65?q=80&w=2070&auto=format&fit=crop')] bg-cover bg-center opacity-10 mix-blend-soft-light" />

        <div className="relative max-w-7xl mx-auto px-6 py-28 lg:py-36 grid lg:grid-cols-2 gap-14 items-center">
          <div>
            <div className="flex flex-col lg:flex-row items-center lg:items-center gap-6 mb-8">
              <img
                src="/logo.png"
                alt="1-7 Church Logo"
                className="w-36 h-36 lg:w-44 lg:h-44 rounded-full object-cover border-4 border-blue-200/60 shadow-[0_0_60px_rgba(59,130,246,0.55)] bg-white/10 p-2 backdrop-blur-md"
              />
              <p className="uppercase tracking-[0.35em] text-2xl lg:text-4xl font-extrabold text-yellow-50 drop-shadow-[0_4px_12px_rgba(0,0,0,0.4)]">
                Welcome to 1-7 Church
              </p>
            </div>
            <h1 className="text-6xl lg:text-8xl xl:text-9xl font-black leading-[0.95] mb-8 drop-shadow-[0_6px_20px_rgba(0,0,0,0.45)] max-w-5xl">
              One Christ, 7 Days, His Glory
            </h1>
            <p className="text-lg text-slate-200 max-w-2xl mb-8 leading-relaxed">
              We are a Christ-centered ministry committed to teaching, worship, prayer, discipleship, outreach, and transforming lives through the power of God’s Word. At 1-7 Church, our passion is to help people encounter Jesus daily, grow in faith, and walk boldly in His purpose every day of the week.
            </p>

            <div className="flex flex-wrap gap-4">
              <button className="bg-white text-slate-900 px-6 py-3 rounded-2xl font-semibold shadow-lg hover:scale-105 transition-transform">
                Plan Your Visit
              </button>
              <button className="border border-white/40 px-6 py-3 rounded-2xl font-semibold hover:bg-white/10 transition-colors">
                Watch Sermons
              </button>
            </div>
          </div>

          <div className="bg-white/15 backdrop-blur-xl rounded-3xl p-8 border border-blue-200/20 shadow-[0_20px_60px_rgba(59,130,246,0.35)]">
            <h2 className="text-3xl font-semibold mb-6">Service Times</h2>

            <div className="space-y-5">
              {services.map((service) => (
                <div
                  key={service.title}
                  className="bg-gradient-to-r from-white/10 to-blue-200/10 rounded-2xl p-5 border border-blue-100/20"
                >
                  <div className="flex items-center justify-between mb-2">
                    <h3 className="font-semibold text-xl">{service.title}</h3>
                    <span className="text-blue-100 text-sm">{service.time}</span>
                  </div>
                  <p className="text-slate-200 text-sm leading-relaxed">
                    {service.description}
                  </p>
                </div>
              ))}
            </div>
          </div>
        </div>
      </section>

      {/* About Section */}
      <section className="max-w-7xl mx-auto px-6 py-24 grid lg:grid-cols-2 gap-16 items-center">
        <div>
          <p className="text-sky-300 font-semibold uppercase tracking-widest mb-3">
            About Us
          </p>
          <h2 className="text-4xl font-bold mb-6 leading-tight text-white">
            A Christ-Centered Ministry Built on Faith, Worship & Truth
          </h2>
          <p className="text-lg text-white leading-relaxed mb-6">
            Our mission is to help people grow spiritually, connect with others,
            and discover their God-given purpose. Through worship gatherings,
            discipleship, outreach, and fellowship, we seek to create a place where
            everyone feels loved and encouraged.
          </p>
          <p className="text-blue-100 leading-relaxed">
            We believe in creating an atmosphere where lives are transformed through
            prayer, biblical teaching, and authentic relationships.
          </p>
        </div>

        <div className="grid grid-cols-2 gap-5">
          {ministries.map((ministry) => (
            <div
              key={ministry}
              className="bg-gradient-to-br from-slate-900/90 to-blue-950/90 rounded-3xl p-6 shadow-lg border border-blue-400/20 hover:shadow-2xl hover:-translate-y-1 transition-all duration-300"
            >
              <div className="text-3xl mb-4">✝️</div>
              <h3 className="font-semibold text-lg text-white">{ministry}</h3>
            </div>
          ))}
        </div>
      </section>

      {/* Vision Section */}
      <section className="bg-[linear-gradient(120deg,#020617_0%,#1d4ed8_35%,#0ea5e9_70%,#312e81_100%)] text-white py-24 px-6">
        <div className="max-w-5xl mx-auto text-center">
          <p className="uppercase tracking-[0.3em] text-indigo-300 mb-4">
            Our Vision
          </p>
          <h2 className="text-4xl lg:text-5xl font-bold mb-8 leading-tight">
            To Reach People, Build Faith, and Impact Generations
          </h2>
          <p className="text-lg text-blue-100 leading-relaxed max-w-3xl mx-auto">
            We are passionate about helping people encounter God, experience genuine
            community, and make a lasting difference in the world around them.
          </p>
        </div>
      </section>

      {/* Contact Section */}
      <section className="max-w-7xl mx-auto px-6 py-24">
        <div className="bg-gradient-to-br from-slate-900/90 to-blue-950/90 rounded-[2rem] shadow-[0_25px_80px_rgba(37,99,235,0.35)] border border-blue-400/20 p-10 lg:p-16 grid lg:grid-cols-2 gap-12">
          <div>
            <p className="uppercase tracking-[0.3em] text-sky-300 mb-3 text-sm">
              Contact Us
            </p>
            <h2 className="text-4xl font-bold mb-6">
              We’d Love to Hear From You
            </h2>
            <p className="text-blue-100 leading-relaxed mb-8">
              Have questions, prayer requests, or want to connect with our ministry?
              Reach out anytime — we’re here for you.
            </p>

            <div className="space-y-4 text-white">
              <p>
                <span className="font-semibold">Email:</span> info@1-7church.org
              </p>
              <p>
                <span className="font-semibold">Phone:</span> (555) 123-4567
              </p>
              <p>
                <span className="font-semibold">Location:</span> Your City, State
              </p>
            </div>
          </div>

          <form className="space-y-5">
            <input
              type="text"
              placeholder="Your Name"
              className="w-full rounded-2xl border border-blue-200/30 bg-white/10 text-white placeholder:text-blue-100 px-5 py-4 focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
            <input
              type="email"
              placeholder="Your Email"
              className="w-full rounded-2xl border border-blue-200/30 bg-white/10 text-white placeholder:text-blue-100 px-5 py-4 focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
            <textarea
              placeholder="Your Message"
              rows={5}
              className="w-full rounded-2xl border border-blue-200/30 bg-white/10 text-white placeholder:text-blue-100 px-5 py-4 focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
            <button
              type="submit"
              className="w-full bg-gradient-to-r from-blue-600 to-sky-500 text-white py-4 rounded-2xl font-semibold hover:scale-[1.02] transition-all shadow-lg"
            >
              Send Message
            </button>
          </form>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-[linear-gradient(90deg,#020617_0%,#1d4ed8_35%,#0ea5e9_70%,#020617_100%)] text-blue-100 py-10 px-6">
        <div className="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-4">
          <div>
            <div className="flex items-center gap-3">
              <img
                src="/logo.png"
                alt="1-7 Church Logo"
                className="w-12 h-12 rounded-full object-cover border border-white/20"
              />
              <h3 className="text-white font-bold text-xl">1-7 Church</h3>
            </div>
            <p className="text-sm mt-1">Faith • Community • Purpose</p>
          </div>

          <div className="text-sm text-center md:text-right">
            <p>© 2026 1-7 Church. All rights reserved.</p>
            <p className="mt-1">Built with faith and purpose.</p>
          </div>
        </div>
      </footer>
    </div>
  );
}
