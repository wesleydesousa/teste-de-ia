import React, { useState } from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Textarea } from "@/components/ui/textarea";
import { Input } from "@/components/ui/input";
import { Select, SelectItem } from "@/components/ui/select";
import { motion } from "framer-motion";

export default function VideoAIApp() {
  const [text, setText] = useState("");
  const [audioFile, setAudioFile] = useState(null);
  const [voiceType, setVoiceType] = useState("normal");
  const [quality, setQuality] = useState("free");
  const [generatedAudio, setGeneratedAudio] = useState(null);
  const [videoUrl, setVideoUrl] = useState(null);
  const [loading, setLoading] = useState(false);
  const [userPlan, setUserPlan] = useState("free");


  // SIMULA BACKEND REAL
  const generateContent = async () => {
    setLoading(true);

    try {
      const response = await fetch("/api/generate", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({ text, voiceType, quality })
      });
      const data = await response.json();


      setGeneratedAudio(data.audio);
      setVideoUrl(data.video);
    } catch (error) {
      console.error(error);
    }


    setLoading(false);
  };

  // SIMULA CHECKOUT STRIPE
  const handleSubscription = async () => {
    alert("Redirecionando para pagamento...");
    setUserPlan("pro");
  };


  return (
    <div className="p-6 grid gap-6">
      <motion.h1
        className="text-3xl font-bold"
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
      >
        🎬 Plataforma SaaS de Vídeos Animados com IA
      </motion.h1>

      {/* STATUS DO USUÁRIO */}
      <Card className="p-4">
        <CardContent>
          <h2 className="font-semibold">Plano Atual: {userPlan.toUpperCase()}</h2>
        </CardContent>
      </Card>


      {/* INPUT */}
      <Card className="p-4">
        <CardContent className="grid gap-4">
          <Textarea
            placeholder="Digite sua história ou roteiro..."
            value={text}
            onChange={(e) => setText(e.target.value)}
          />

          <Input
            type="file"
            accept="audio/*"
            onChange={(e) => setAudioFile(e.target.files[0])}
          />

          <Select onValueChange={setVoiceType}>
            <SelectItem value="normal">Voz Normal (Free)</SelectItem>
            <SelectItem value="premium">Voz Ultra Realista (Pro)</SelectItem>
          </Select>

          <Select onValueChange={setQuality}>
            <SelectItem value="free">HD com Marca</SelectItem>
            <SelectItem value="pro">Full HD sem Marca</SelectItem>
          </Select>

          <Button onClick={generateContent} disabled={loading}>
            {loading ? "Gerando IA..." : "Gerar Vídeo"}
          </Button>
        </CardContent>
      </Card>

      {/* RESULTADOS */}
      {generatedAudio && (
        <Card className="p-4">
          <CardContent>
            <h2>🔊 Áudio</h2>
            <audio controls src={generatedAudio}></audio>
          </CardContent>
        </Card>
      )}

      {videoUrl && (
        <Card className="p-4">
          <CardContent>
            <h2>📺 Vídeo Gerado</h2>
            <video controls className="w-full rounded-xl" src={videoUrl}></video>
            <Button className="mt-3">📥 Baixar Vídeo</Button>
          </CardContent>
        </Card>
      )}


      {/* MONETIZAÇÃO */}
      {userPlan === "free" && (
        <Card className="p-4 bg-green-100">
          <CardContent className="flex justify-between items-center">
            <div>
              <h2 className="font-semibold">🚀 Upgrade para PRO</h2>
              <p>Remova a marca d'água + voz realista</p>
            </div>
            <Button onClick={handleSubscription}>Assinar R$29/mês</Button>
          </CardContent>
        </Card>
      )}


      {/* PREVIEW ANIMADO */}
      {!videoUrl && (
        <Card className="p-4">
          <CardContent>
            <h2>Preview</h2>
            <div className="w-full h-64 bg-blue-200 flex items-center justify-center rounded-2xl">
              <motion.div
                animate={{ y: [0, -20, 0] }}
                transition={{ repeat: Infinity, duration: 1.2 }}
                className="text-xl"
              >
                🏊‍♂️ Personagem Nadando
              </motion.div>
            </div>
          </CardContent>
        </Card>
      )}
    </div>
  );
}

// ================= BACKEND EXEMPLO (Node.js) =================

/*

// server.js
import express from "express";
import cors from "cors";

const app = express();
app.use(cors());
app.use(express.json());

app.post("/api/generate", async (req, res) => {
  const { text } = req.body;

  // Aqui você integraria:
  // - OpenAI (roteiro)
  // - ElevenLabs (voz)
  // - Remotion (vídeo)

  return res.json({
    audio: "/audio-gerado.mp3",
    video: "/video-gerado.mp4"
  });
});

app.listen(3001, () => console.log("Servidor rodando"));

*/
