import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { motion } from "framer-motion";

export default function Portfolio() {
  return (
    <main className="min-h-screen bg-black text-white px-4 md:px-12 py-10">
      <section className="text-center mb-12">
        <h1 className="text-4xl md:text-5xl font-bold text-gradient mb-4">
          Shruthi Reddy Vudem
        </h1>
        <p className="text-lg md:text-xl text-gray-300">
          Health Data Scientist | Machine Learning Enthusiast | Research-Driven Thinker
        </p>
      </section>

      <motion.section
        initial={{ opacity: 0, y: 40 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.6 }}
        className="grid md:grid-cols-2 gap-8"
      >
        <Card className="bg-gray-900 border border-gray-700">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-white mb-2">About Me</h2>
            <p className="text-gray-300 text-sm">
              I’m a data scientist with a foundation in healthcare, machine learning, and research. Passionate about
              turning clinical and societal data into actionable insights through statistical modeling and
              visualization.
            </p>
          </CardContent>
        </Card>

        <Card className="bg-gray-900 border border-gray-700">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-white mb-2">Projects</h2>
            <ul className="list-disc pl-5 text-gray-300 text-sm">
              <li>Excelerate Insights Dashboard – Tech career visualizations in Looker Studio</li>
              <li>Parkinson’s Data Dashboard – Balance perception analysis in PD</li>
              <li>Drug Death Prediction – ML pipeline with Dask + Random Forest</li>
              <li>SAR Ride Cancellation – Multi-model ML classification</li>
            </ul>
          </CardContent>
        </Card>

        <Card className="bg-gray-900 border border-gray-700">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-white mb-2">Research</h2>
            <p className="text-gray-300 text-sm">
              Published in IJECSE – Open Apex Management (2022). Current work: Fall risk in Parkinson’s Disease using
              UPDRS, Mini-BESTest, and PDQ-39 metrics.
            </p>
          </CardContent>
        </Card>

        <Card className="bg-gray-900 border border-gray-700">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-white mb-2">Certifications</h2>
            <ul className="list-disc pl-5 text-gray-300 text-sm">
              <li>Machine Learning with Python – IBM/LinkedIn</li>
              <li>Tableau Essential Training – LinkedIn Learning</li>
              <li>Human Research – CITI Program</li>
              <li>Clinical Decision Making – Cleveland Clinic</li>
            </ul>
          </CardContent>
        </Card>
      </motion.section>

      <section className="text-center mt-12">
        <Button className="bg-pink-600 hover:bg-pink-700 text-white px-6 py-2 text-lg rounded-2xl">
          <a href="/VSR_RESUMEZ_F.pdf" target="_blank" rel="noopener noreferrer">
            Download Resume
          </a>
        </Button>
      </section>
    </main>
  );
}
