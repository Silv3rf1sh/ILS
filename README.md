# ILS
Website?
import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { FaShippingFast, FaWarehouse, FaChartLine, FaUsers } from "react-icons/fa";

export default function ILSHomePage() {
  return (
    <div className="bg-black text-ivory min-h-screen">
      {/* Navigation Bar */}
      <header className="flex justify-between items-center p-6 border-b border-wine fixed w-full bg-black z-50">
        <h1 className="text-2xl font-bold">ILS</h1>
        <nav className="space-x-6 hidden md:flex">
          <a href="#solutions" className="hover:text-wine">Solutions</a>
          <a href="#about" className="hover:text-wine">About</a>
          <a href="#case-studies" className="hover:text-wine">Case Studies</a>
          <a href="#contact" className="hover:text-wine">Contact</a>
        </nav>
        <Button className="bg-wine text-black px-4 py-2">Request a Demo</Button>
      </header>

      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center h-screen text-center px-6 bg-opacity-90">
        <h2 className="text-5xl font-bold">Revolutionizing Supply Chains with AI & Automation</h2>
        <p className="text-lg mt-4">Optimize Logistics, Reduce Costs, and Improve Efficiency</p>
        <div className="mt-6 space-x-4">
          <Button className="bg-wine text-black px-6 py-3">Request a Demo</Button>
          <Button variant="outline" className="border-wine text-wine px-6 py-3">Learn More</Button>
        </div>
      </section>

      {/* Key Features Section */}
      <section id="solutions" className="p-12 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
        <Card className="bg-opacity-10 hover:bg-opacity-20 border border-wine">
          <CardContent className="flex flex-col items-center p-6">
            <FaChartLine className="text-wine text-4xl" />
            <h3 className="text-xl font-semibold mt-4">AI-Powered Optimization</h3>
            <p className="text-center text-sm">Smarter forecasting and decision-making.</p>
          </CardContent>
        </Card>
        <Card className="bg-opacity-10 hover:bg-opacity-20 border border-wine">
          <CardContent className="flex flex-col items-center p-6">
            <FaShippingFast className="text-wine text-4xl" />
            <h3 className="text-xl font-semibold mt-4">IoT & Real-Time Tracking</h3>
            <p className="text-center text-sm">Live visibility into inventory & shipments.</p>
          </CardContent>
        </Card>
        <Card className="bg-opacity-10 hover:bg-opacity-20 border border-wine">
          <CardContent className="flex flex-col items-center p-6">
            <FaWarehouse className="text-wine text-4xl" />
            <h3 className="text-xl font-semibold mt-4">Automated Warehousing</h3>
            <p className="text-center text-sm">Reduce manual errors with AI-driven processes.</p>
          </CardContent>
        </Card>
        <Card className="bg-opacity-10 hover:bg-opacity-20 border border-wine">
          <CardContent className="flex flex-col items-center p-6">
            <FaUsers className="text-wine text-4xl" />
            <h3 className="text-xl font-semibold mt-4">Smart Vendor Auctions</h3>
            <p className="text-center text-sm">Secure, transparent procurement using blockchain.</p>
          </CardContent>
        </Card>
      </section>

      {/* Contact Form */}
      <section id="contact" className="p-12 text-center">
        <h3 className="text-3xl font-semibold">Contact Us</h3>
        <p className="text-sm mt-2">Have questions? Get in touch with us.</p>
        <div className="mt-6 max-w-md mx-auto">
          <Input className="mb-4" placeholder="Your Name" />
          <Input className="mb-4" placeholder="Your Email" />
          <Textarea className="mb-4" placeholder="Your Message" />
          <Button className="bg-wine text-black px-6 py-3">Submit Inquiry</Button>
        </div>
      </section>

      {/* Footer */}
      <footer className="p-6 text-center border-t border-wine mt-12">
        <p>© 2025 ILS. All Rights Reserved.</p>
      </footer>
    </div>
  );
}
