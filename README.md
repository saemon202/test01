import React from "react";

export default function LandingPage() {
  return (
    <div className="relative w-full min-h-screen text-white">
      {/* Background Video */}
      <video
        autoPlay
        muted
        loop
        className="absolute w-full h-full object-cover z-0"
      >
        <source src="/videos/business-transition.mp4" type="video/mp4" />
      </video>

      <div className="relative z-10 flex flex-col lg:flex-row items-center justify-between p-10 lg:p-20 gap-10 bg-black/60 min-h-screen">
        {/* Hero Text */}
        <div className="max-w-xl space-y-6">
          <h1 className="text-4xl lg:text-6xl font-bold">
            Ready to Sell Your Business? We’ll Guide You Every Step of the Way.
          </h1>
          <p className="text-lg lg:text-xl">
            Fitzwilliams Financial helps business owners like you get the most out of their hard work — from valuation to final sale.
          </p>
        </div>

        {/* Form */}
        <form className="bg-white text-black p-6 rounded-2xl shadow-lg w-full max-w-md space-y-4">
          <h2 className="text-2xl font-semibold">Get a Free Consultation</h2>
          <input type="text" placeholder="Name" className="w-full p-3 rounded border" />
          <input type="email" placeholder="Email" className="w-full p-3 rounded border" />
          <input type="tel" placeholder="Phone" className="w-full p-3 rounded border" />
          <button className="w-full bg-blue-600 text-white py-3 rounded-xl hover:bg-blue-700">
            Submit
          </button>
        </form>
      </div>

      {/* Learn Section */}
      <section className="bg-white text-black p-10 space-y-6">
        <h2 className="text-3xl font-bold">You Will Learn About</h2>
        <ul className="list-disc pl-6 space-y-2">
          <li>How much your business is worth</li>
          <li>How to structure a sale for maximum value</li>
          <li>Common mistakes to avoid when selling</li>
          <li>What buyers are really looking for</li>
        </ul>
        <button className="mt-4 bg-blue-600 text-white py-2 px-4 rounded-xl hover:bg-blue-700">
          Speak With an Advisor
        </button>
      </section>

      {/* Testimonials */}
      <section className="bg-gray-100 text-black p-10 space-y-6">
        <h2 className="text-3xl font-bold">Real Succession Stories</h2>
        <div className="space-y-4">
          <blockquote className="bg-white p-4 rounded-xl shadow">
            <p className="italic">“I didn’t know where to begin. They walked me through every step.”</p>
            <footer className="mt-2 font-semibold">— John P., Plumbing Company Owner</footer>
          </blockquote>
          <blockquote className="bg-white p-4 rounded-xl shadow">
            <p className="italic">“They got me more than I thought my business was worth.”</p>
            <footer className="mt-2 font-semibold">— Linda R., Retail Franchise Owner</footer>
          </blockquote>
        </div>
      </section>

      {/* FAQ */}
      <section className="bg-white text-black p-10 space-y-6">
        <h2 className="text-3xl font-bold">FAQ</h2>
        <div className="space-y-4">
          <div>
            <strong>How long does the process take?</strong>
            <p>Most of our clients complete the sale within 3–9 months.</p>
          </div>
          <div>
            <strong>Do I need to have my financials perfectly in order?</strong>
            <p>No, we’ll help you prepare and clean up anything that needs work.</p>
          </div>
          <div>
            <strong>How do you find buyers?</strong>
            <p>We maintain a private network of pre-qualified buyers and also market strategically when needed.</p>
          </div>
        </div>
      </section>

      {/* Bottom CTA */}
      <section className="bg-blue-800 text-white p-10 text-center space-y-6">
        <h2 className="text-3xl font-bold">Thinking of Selling in the Next 12 Months?</h2>
        <p>Start with a no-pressure, confidential conversation. You’ve built it — we’ll help you exit smart.</p>
        <button className="bg-white text-blue-800 py-3 px-6 rounded-xl hover:bg-gray-200">
          Book My Free Consultation
        </button>
      </section>
    </div>
  );
}
