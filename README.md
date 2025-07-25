import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import Link from "next/link";

export default function DrStrongWebsite() {
  return (
    <div className="p-6 space-y-10">
      {/* Navigation Bar */}
      <nav className="flex justify-between items-center py-4 border-b">
        <h1 className="text-2xl font-bold">Dr.Strong</h1>
        <ul className="flex gap-6 text-lg">
          <li><Link href="#how-it-works">How It Works</Link></li>
          <li><Link href="#for-clients">Clients</Link></li>
          <li><Link href="#for-trainers">Trainers</Link></li>
          <li><Link href="#clinic-network">Clinics</Link></li>
          <li><Link href="#education">Education</Link></li>
          <li><Link href="#contact">Contact</Link></li>
        </ul>
      </nav>

      {/* Hero Section */}
      <section className="text-center space-y-4 mt-10">
        <h2 className="text-4xl font-bold">Empowering Safe, Scientific Body Transformation</h2>
        <p className="text-lg max-w-2xl mx-auto">
          Welcome to Dr.Strong — a medically guided ecosystem for fat loss, muscle gain, and sustainable body transformation.
        </p>
      </section>

      {/* Cards Section */}
      <section className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-10">
        <Card id="how-it-works">
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold">How It Works</h2>
            <p>
              Doctor-led programs, trainer partnerships, and a clinic network ensure results through a 360° transformation model.
            </p>
          </CardContent>
        </Card>
        <Card id="for-clients">
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold">For Clients</h2>
            <p>
              Get a personalized transformation roadmap with medical screening, tailored programs, and live monitoring.
            </p>
          </CardContent>
        </Card>
        <Card id="for-trainers">
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold">For Trainers</h2>
            <p>
              Retain your clients and boost results with medically supported programs, compliance tools, and co-branded assets.
            </p>
          </CardContent>
        </Card>
        <Card id="clinic-network">
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold">Clinic Network</h2>
            <p>
              100+ clinics collaborate with Dr.Strong for patient referrals, cross-promotion, and certified transformation programs.
            </p>
          </CardContent>
        </Card>
        <Card id="education">
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold">Education Hub</h2>
            <p>
              Stay up to date with monthly seminars, expert modules, and Dr.Strong certifications for doctors and trainers.
            </p>
          </CardContent>
        </Card>
        <Card>
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold">Join Us</h2>
            <p>
              Be part of the trusted ecosystem — onboard as a trainer, clinic, or client today.
            </p>
          </CardContent>
        </Card>
      </section>

      {/* Contact Section */}
      <section id="contact" className="text-center mt-16 space-y-4">
        <h2 className="text-2xl font-bold">Contact Us</h2>
        <p>Have questions? Reach out and we’ll guide you through your transformation journey.</p>
        <Button className="text-lg">Get in Touch</Button>
      </section>
    </div>
  );
}
