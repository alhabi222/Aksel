# Aksel
# Panduan Proposal & Kode Sumber Proyek AkselAI - BI-OJK Hackathon 2025

Dokumen ini berisi dua bagian:
1.  **Panduan Proposal:** Kerangka kerja untuk menyusun presentasi (deck) Anda.
2.  **Kode Sumber Lengkap:** Salinan lengkap dari semua file kode penting proyek AkselAI.

---
## BAGIAN 1: PANDUAN PROPOSAL
---

**Slide 1: Halaman Judul**
- **Tulisan:** Proposal BI-OJK Hackathon 2025
- **Judul Proyek:** AkselAI: Platform AI-sebagai-Layanan (AIaaS) untuk Akselerasi Inovasi Keuangan dan Layanan Publik
- **Nama Tim:** [Aksel]
- **Nama Anggota:** [Nama Lengkap Anda]

**Slide 2: Ringkasan Eksekutif (Maks. 1 slide)**
- **Problem Statement:** Di tengah ledakan AI, banyak institusi keuangan, UMKM, dan lembaga pemerintah masih kesulitan membangun solusi AI yang spesifik untuk kebutuhan unik mereka. Mereka terjebak antara solusi generik yang tidak efektif atau biaya pengembangan kustom yang sangat mahal. Akibatnya, potensi AI untuk meningkatkan literasi keuangan, daya saing UMKM, dan efisiensi layanan publik belum termanfaatkan sepenuhnya.
- **Solusi Kami:** AkselAI adalah platform AI-sebagai-Layanan (AIaaS) yang memberdayakan siapa saja—mulai dari bank hingga developer individu—untuk **membangun, melatih, dan men-deploy Partner AI khusus** tanpa memerlukan tim AI yang besar. Kami mengubah paradigma dari sekadar *menggunakan* AI menjadi *menciptakan* solusi AI.
- **Dampak Positif:** AkselAI secara langsung mendukung tema Hackathon dengan menjadi **akselerator inovasi**. Platform kami memungkinkan penciptaan layanan ekspor digital (Sub-tema 1), solusi literasi keuangan dan UMKM (Sub-tema 2), serta alat bantu analisis risiko (Sub-tema 3) dengan cepat dan efisien, mendorong pertumbuhan inklusif dan ekonomi yang tangguh.

**Slide 3: Anggota Tim (Maks. 1 slide)**
- **Nama Lengkap:** [Nama Anda]
- **Kontak:** [Nomor Telepon/WA Anda]
- **Email:** rgomet48@gmail.com
- **Peran dalam tim:** Lead Developer & AI Architect
- **Keahlian:** Full-stack development dengan Next.js & TypeScript, arsitektur dan implementasi solusi AI generatif menggunakan Google Genkit, perancangan UI/UX, dan product strategy.
- **Link Portofolio:** [Link ke Repositori GitHub Proyek Ini]

**Slide 4: Tujuan/Sasaran Proyek (Maks. 1 slide)**
- **Tujuan Utama:** Mendemokratisasi akses pengembangan solusi AI di sektor keuangan dan layanan publik Indonesia.
- **Sasaran Terukur:**
  1. Menyediakan platform yang dapat mengurangi waktu pengembangan prototipe AI dari bulan menjadi hari.
  2. Menghasilkan minimal 3 PoC (Proof of Concept) Partner AI yang relevan dengan sub-tema BI-OJK Hackathon (e.g., Cerdas Keuangan, UMKM Maju, BlockGuardian).
  3. Menciptakan model bisnis B2B subscription yang berkelanjutan dan terukur.
- **Dampak:**
  - **Untuk Ekonomi Digital:** Mempercepat lahirnya startup dan layanan digital baru berbasis AI.
  - **Untuk BI & OJK:** Menyediakan alat bagi industri di bawah pengawasan BI/OJK untuk berinovasi secara bertanggung jawab, meningkatkan literasi keuangan, dan memperkuat manajemen risiko.

**Slide 5: Rumusan Masalah (Maks. 1 slide)**
- **Masalah:** Kesenjangan Inovasi AI. Lembaga keuangan dan pemerintah tahu mereka butuh AI, tetapi (1) solusi yang ada terlalu umum, (2) membuat solusi sendiri terlalu mahal dan lambat, dan (3) talenta AI masih langka.
- **Solusi yang Ada Tidak Memadai:** Chatbot generik tidak memahami konteks keuangan atau regulasi Indonesia. Proyek AI kustom memakan waktu berbulan-bulan dan miliaran rupiah.
- **Pendekatan Baru Kami:** AkselAI menawarkan jalan tengah yang revolusioner. Kami bukan produk, kami adalah **platform**. Aspek baru kami adalah **pemberdayaan**; kami memberikan kemampuan AI canggih ke tangan para inovator di semua tingkatan. Fitur **evolusi partner** kami juga memastikan solusi AI dapat terus beradaptasi dan menjadi lebih pintar seiring waktu.

**Slide 6-7: Metode/Mekanisme AI/ML & Blockchain (2-3 slide)**
- **Slide 6: Arsitektur Umum**
  - **Diagram Alur:** [Pengguna] -> [Frontend Next.js] -> [Backend Genkit Flow] -> [Google Gemini Model API].
  - **Rancangan Solusi:** AkselAI adalah aplikasi web berbasis Next.js yang berinteraksi dengan serangkaian alur kerja AI (Genkit Flows) di sisi server. Setiap "Partner AI" pada dasarnya adalah Genkit Flow yang dikonfigurasi dengan *system prompt*, *input/output schema* (menggunakan Zod), dan *tools* yang spesifik untuk keahliannya.
  - **Contoh:** Partner "Cerdas Keuangan" memiliki *system prompt* yang memerintahkannya untuk berperan sebagai penasihat keuangan dan menggunakan skema output yang terstruktur untuk memberikan saran anggaran.
- **Slide 7: Penggunaan AI/ML & Blockchain secara Teknis**
  - **AI/ML:** Kami menggunakan **Google Gemini 1.5 Flash** melalui **Genkit Framework**.
    - **Algoritma:** Ini adalah model bahasa besar (LLM) multimodal. Kami tidak membangun model dari nol, melainkan melakukan *prompt engineering* dan *structured output formatting* untuk mengarahkan LLM agar berfungsi sebagai ahli di domain tertentu. Ini adalah pendekatan AIaaS yang paling efisien.
    - **Keunggulan Genkit:** Memungkinkan kami mendefinisikan alur yang andal, dapat diuji, dan dipantau, yang sangat penting untuk keandalan di sektor keuangan.
  - **Blockchain (sebagai *Use Case*, bukan *Core Tech*):** Kami menunjukkan fleksibilitas platform dengan Partner AI **"BlockGuardian"**.
    - **Mekanisme:** Partner ini menggunakan AI untuk **menganalisis kode smart contract (dalam bentuk teks) dan mendeteksi pola-pola kerentanan umum** berdasarkan basis pengetahuan yang telah dilatih pada LLM. Ini adalah penggunaan AI untuk *meningkatkan keamanan* ekosistem blockchain, bukan sekadar menggunakan blockchain demi tren.

**Slide 8: Dataset yang Digunakan (Maks 2 slide)**
- **Slide 8.1: Pendekatan Dataset Modern:**
  - **Jenis Dataset:** Kami tidak menggunakan dataset statis. "Dataset" kami adalah **pengetahuan fundamental dari Google Gemini 1.5 Flash**, yang dilatih pada data global yang luas.
  - **Sumber Dataset:** Dataset pre-training milik Google menjadi dasar pengetahuan AI kami.
- **Slide 8.2: Kualitas dan Keandalan melalui Prompt Engineering:**
  - Kami tidak *membersihkan* dataset, kami *mengarahkan* model. Kualitas dipastikan melalui:
    1.  **System Prompt Engineering:** Setiap Partner AI memiliki peran dan batasan yang jelas.
    2.  **Structured Output (Zod Schema):** Kami memaksa AI memberikan respons dalam format JSON yang tervalidasi, memastikan konsistensi.
    3.  **Evolusi Berbasis Interaksi:** Fitur evolusi memungkinkan partner belajar dari interaksi, mensimulasikan pembelajaran dari data baru.

**Slide 9: Tools dan Teknologi yang Digunakan (Max 1 slide)**
- **Tools & Teknologi:**
  - **Frontend:** Next.js, React, TypeScript, ShadCN UI, Tailwind CSS.
  - **Backend & AI:** Google Genkit Framework.
  - **Model AI:** Google Gemini 1.5 Flash.
  - **Authentication:** Firebase Auth.
- **Alasan Pemilihan:**
  - **Next.js:** Memberikan performa tinggi dan pengalaman pengguna yang modern.
  - **Google Genkit:** Dipilih karena menyediakan kerangka kerja yang tangguh (*robust*) untuk membangun alur kerja AI yang dapat dipantau dan siap produksi, krusial untuk sektor keuangan.
  - **Gemini 1.5 Flash:** Menawarkan kecepatan, kemampuan multimodal, dan efisiensi biaya.

**Slide 10: Bisnis Model & Keberlanjutan (Gunakan Business Model Canvas)**
- **Customer Segments:** Bank, Lembaga Keuangan, Perusahaan Fintech, Instansi Pemerintah.
- **Value Propositions:** Akselerasi inovasi AI, pengurangan biaya R&D, penciptaan layanan keuangan baru.
- **Revenue Streams:** Langganan berjenjang (Tier Basic, Pro, Enterprise) untuk akses platform.
- **Cost Structure:** Biaya API Google Gemini, biaya hosting, biaya pengembangan.
- **Key Activities:** Pengembangan platform, riset prompt engineering, pemasaran.
- **Key Partnerships:** Google (penyedia teknologi AI), Bank Indonesia & OJK (regulator & potential user).

**Slide 11: Rancangan Mockup, POC, Prototype (Max 3 slide)**
- **Slide 11.1: Prototipe Fungsional:** Tampilkan screenshot dari aplikasi AkselAI yang berjalan (halaman utama).
- **Slide 11.2: PoC - Solusi Keuangan:** Tampilkan screenshot interaksi dengan Partner **"Cerdas Keuangan"** atau **"UMKM Maju"**.
- **Slide 11.3: PoC - Keamanan Blockchain:** Tampilkan screenshot interaksi dengan Partner **"BlockGuardian"**.

**Slide 12: Penutup (Max 1 slide)**
- Rangkum visi AkselAI: Bukan hanya produk, tetapi **akselerator ekosistem inovasi AI di Indonesia**.
- Ucapkan terima kasih.

---
## BAGIAN 2: KODE SUMBER LENGKAP
---

### PETUNJUK
Untuk mereplikasi proyek ini, buat proyek Next.js baru, lalu salin konten setiap file di bawah ini dan buat file baru dengan nama yang sesuai di dalam proyek Anda.

---
### `package.json`
```json
{
  "name": "nextn",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "dev": "dotenv -e src/ai/.env -- next dev -p 9002",
    "genkit:dev": "dotenv -e src/ai/.env -- genkit start -- tsx src/ai/dev.ts",
    "genkit:watch": "dotenv -e src/ai/.env -- genkit start -- tsx --watch src/ai/dev.ts",
    "build": "next build",
    "start": "next start",
    "lint": "next lint",
    "typecheck": "tsc --noEmit",
    "deploy": "firebase deploy --only hosting"
  },
  "dependencies": {
    "@genkit-ai/googleai": "^1.13.0",
    "@genkit-ai/next": "^1.13.0",
    "@hookform/resolvers": "^4.1.3",
    "@opentelemetry/exporter-jaeger": "^1.25.1",
    "@radix-ui/react-accordion": "^1.2.3",
    "@radix-ui/react-alert-dialog": "^1.1.6",
    "@radix-ui/react-avatar": "^1.1.3",
    "@radix-ui/react-checkbox": "^1.1.4",
    "@radix-ui/react-collapsible": "^1.1.11",
    "@radix-ui/react-dialog": "^1.1.6",
    "@radix-ui/react-dropdown-menu": "^2.1.6",
    "@radix-ui/react-label": "^2.1.2",
    "@radix-ui/react-menubar": "^1.1.6",
    "@radix-ui/react-popover": "^1.1.6",
    "@radix-ui/react-progress": "^1.1.2",
    "react-hook-form": "^7.54.2",
    "@radix-ui/react-radio-group": "^1.2.3",
    "@radix-ui/react-scroll-area": "^1.2.3",
    "@radix-ui/react-select": "^2.1.6",
    "@radix-ui/react-separator": "^1.1.2",
    "@radix-ui/react-slider": "^1.2.3",
    "@radix-ui/react-slot": "^1.2.3",
    "@radix-ui/react-switch": "^1.1.3",
    "@radix-ui/react-tabs": "^1.1.3",
    "@radix-ui/react-toast": "^1.2.6",
    "@radix-ui/react-tooltip": "^1.1.8",
    "class-variance-authority": "^0.7.1",
    "clsx": "^2.1.1",
    "date-fns": "^3.6.0",
    "dotenv": "^16.4.5",
    "embla-carousel-react": "^8.6.0",
    "firebase": "^11.9.1",
    "genkit": "^1.13.0",
    "lucide-react": "^0.475.0",
    "next": "latest",
    "react": "^18.3.1",
    "react-day-picker": "^8.10.1",
    "react-dom": "^18.3.1",
    "recharts": "^2.15.1",
    "tailwind-merge": "^3.0.1",
    "tailwindcss-animate": "^1.0.7",
    "zod": "^3.24.2"
  },
  "devDependencies": {
    "@types/node": "^20",
    "@types/react": "^18",
    "@types/react-dom": "^18",
    "cross-env": "^7.0.3",
    "dotenv-cli": "^7.4.2",
    "firebase-tools": "^13.14.2",
    "genkit-cli": "^1.13.0",
    "postcss": "^8",
    "tailwindcss": "^3.4.1",
    "typescript": "^5"
  }
}
```

---
### `tailwind.config.ts`
```ts
import type {Config} from 'tailwindcss';

export default {
  darkMode: ['class'],
  content: [
    './src/pages/**/*.{js,ts,jsx,tsx,mdx}',
    './src/components/**/*.{js,ts,jsx,tsx,mdx}',
    './src/app/**/*.{js,ts,jsx,tsx,mdx}',
  ],
  theme: {
    container: {
      center: true,
      padding: "2rem",
      screens: {
        "2xl": "1400px",
      },
    },
    extend: {
      fontFamily: {
        body: ['Inter', 'sans-serif'],
        headline: ['"Space Grotesk"', 'sans-serif'],
        code: ['monospace'],
      },
      colors: {
        background: 'hsl(var(--background))',
        foreground: 'hsl(var(--foreground))',
        card: {
          DEFAULT: 'hsl(var(--card))',
          foreground: 'hsl(var(--card-foreground))',
        },
        popover: {
          DEFAULT: 'hsl(var(--popover))',
          foreground: 'hsl(var(--popover-foreground))',
        },
        primary: {
          DEFAULT: 'hsl(var(--primary))',
          foreground: 'hsl(var(--primary-foreground))',
        },
        secondary: {
          DEFAULT: 'hsl(var(--secondary))',
          foreground: 'hsl(var(--secondary-foreground))',
        },
        muted: {
          DEFAULT: 'hsl(var(--muted))',
          foreground: 'hsl(var(--muted-foreground))',
        },
        accent: {
          DEFAULT: 'hsl(var(--accent))',
          foreground: 'hsl(var(--accent-foreground))',
        },
        destructive: {
          DEFAULT: 'hsl(var(--destructive))',
          foreground: 'hsl(var(--destructive-foreground))',
        },
        border: 'hsl(var(--border))',
        input: 'hsl(var(--input))',
        ring: 'hsl(var(--ring))',
        chart: {
          '1': 'hsl(var(--chart-1))',
          '2': 'hsl(var(--chart-2))',
          '3': 'hsl(var(--chart-3))',
          '4': 'hsl(var(--chart-4))',
          '5': 'hsl(var(--chart-5))',
        },
        sidebar: {
          DEFAULT: 'hsl(var(--sidebar-background))',
          foreground: 'hsl(var(--sidebar-foreground))',
          primary: 'hsl(var(--sidebar-primary))',
          'primary-foreground': 'hsl(var(--sidebar-primary-foreground))',
          accent: 'hsl(var(--sidebar-accent))',
          'accent-foreground': 'hsl(var(--sidebar-accent-foreground))',
          border: 'hsl(var(--sidebar-border))',
          ring: 'hsl(var(--sidebar-ring))',
        },
      },
      borderRadius: {
        lg: 'var(--radius)',
        md: 'calc(var(--radius) - 2px)',
        sm: 'calc(var(--radius) - 4px)',
      },
      keyframes: {
        'accordion-down': {
          from: {
            height: '0',
          },
          to: {
            height: 'var(--radix-accordion-content-height)',
          },
        },
        'accordion-up': {
          from: {
            height: 'var(--radix-accordion-content-height)',
          },
          to: {
            height: '0',
          },
        },
      },
      animation: {
        'accordion-down': 'accordion-down 0.2s ease-out',
        'accordion-up': 'accordion-up 0.2s ease-out',
      },
    },
  },
  plugins: [require('tailwindcss-animate')],
} satisfies Config;
```

---
### `src/app/globals.css`
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  :root {
    --background: 0 0% 100%;
    --foreground: 222.2 84% 4.9%;
    --card: 0 0% 100%;
    --card-foreground: 222.2 84% 4.9%;
    --popover: 0 0% 100%;
    --popover-foreground: 222.2 84% 4.9%;
    --primary: 222.2 47.4% 11.2%;
    --primary-foreground: 210 40% 98%;
    --secondary: 210 40% 96.1%;
    --secondary-foreground: 222.2 47.4% 11.2%;
    --muted: 210 40% 96.1%;
    --muted-foreground: 215.4 16.3% 46.9%;
    --accent: 344 29% 57%;
    --accent-foreground: 210 40% 98%;
    --destructive: 0 84.2% 60.2%;
    --destructive-foreground: 210 40% 98%;
    --border: 214.3 31.8% 91.4%;
    --input: 214.3 31.8% 91.4%;
    --ring: 222.2 84% 4.9%;
    --radius: 0.5rem;
    --chart-1: 12 76% 61%;
    --chart-2: 173 58% 39%;
    --chart-3: 197 37% 24%;
    --chart-4: 43 74% 66%;
    --chart-5: 27 87% 67%;
    --sidebar-background: 211 33% 18%;
    --sidebar-foreground: 210 40% 98%;
    --sidebar-primary: 344 29% 57%;
    --sidebar-primary-foreground: 0 0% 100%;
    --sidebar-accent: 210 30% 30%;
    --sidebar-accent-foreground: 210 40% 98%;
    --sidebar-border: 210 30% 30%;
    --sidebar-ring: 344 29% 57%;
  }
 
  .dark {
    --background: 211 33% 18%;
    --foreground: 210 40% 98%;
    --card: 210 35% 22%;
    --card-foreground: 210 40% 98%;
    --popover: 211 33% 18%;
    --popover-foreground: 210 40% 98%;
    --primary: 209 39% 35%;
    --primary-foreground: 210 40% 98%;
    --secondary: 210 30% 30%;
    --secondary-foreground: 210 40% 98%;
    --muted: 210 30% 30%;
    --muted-foreground: 210 40% 60%;
    --accent: 344 29% 57%;
    --accent-foreground: 0 0% 100%;
    --destructive: 0 63% 31%;
    --destructive-foreground: 210 40% 98%;
    --border: 210 30% 30%;
    --input: 210 30% 30%;
    --ring: 344 29% 57%;
    --chart-1: 220 70% 50%;
    --chart-2: 160 60% 45%;
    --chart-3: 30 80% 55%;
    --chart-4: 280 65% 60%;
    --chart-5: 340 75% 55%;
    --sidebar-background: 211 33% 18%;
    --sidebar-foreground: 210 40% 98%;
    --sidebar-primary: 344 29% 57%;
    --sidebar-primary-foreground: 0 0% 100%;
    --sidebar-accent: 210 30% 30%;
    --sidebar-accent-foreground: 210 40% 98%;
    --sidebar-border: 210 30% 30%;
    --sidebar-ring: 344 29% 57%;
  }
}

@layer base {
  * {
    @apply border-border;
  }
  body {
    @apply bg-background text-foreground;
  }
}
```

---
### `src/app/layout.tsx`
```tsx
import type { Metadata } from 'next';
import './globals.css';

export const metadata: Metadata = {
  title: 'AkselAI: Custom AI Partners for Skill Acceleration',
  description: 'Build, train, and collaborate with specialized AI partners. AkselAI helps you accelerate your expertise in any field, from coding and writing to business strategy.',
};

export default function RootLayout({
  children,
}: Readonly<{
  children: React.ReactNode;
}>) {
  return (
    <html lang="en" className="dark" suppressHydrationWarning>
      <head>
        <link rel="preconnect" href="https://fonts.googleapis.com" />
        <link rel="preconnect" href="https://fonts.gstatic.com" crossOrigin="anonymous" />
        <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet" />
      </head>
      <body className="font-body antialiased">
        {children}
      </body>
    </html>
  );
}
```

---
### `src/app/(app)/page.tsx`
```tsx
'use client';

import { useEffect, useState } from 'react';
import { Loader2, PlusCircle, RotateCcw } from 'lucide-react';
import { useAuth } from '@/hooks/use-auth';
import { usePartners } from '@/hooks/use-partners';
import { useRouter } from 'next/navigation';
import { FeedbackCard } from '@/components/feedback-card';
import { PartnerCard } from '@/components/partner-card';
import { Button } from '@/components/ui/button';
import { CreatePartnerDialog } from '@/components/create-partner-dialog';
import { ClientOnly } from '@/components/client-only';
import { StrategicAdvisorCard } from '@/components/strategic-advisor-card';

export default function HomePage() {
  const { user, loading, isTrialActive } = useAuth();
  const { partners, deletePartner, resetPartners, addPartner } = usePartners();
  const router = useRouter();
  const [isCreateDialogOpen, setCreateDialogOpen] = useState(false);

  useEffect(() => {
    if (!loading && !user) {
      router.push('/login');
    }
  }, [user, loading, router]);

  if (loading || !user) {
    return (
      <div className="flex h-screen w-full items-center justify-center">
        <Loader2 className="h-8 w-8 animate-spin text-accent" />
      </div>
    );
  }

  return (
    <>
      <div className="container mx-auto p-4 sm:p-6 lg:p-8">
        <div className="mb-8">
          <div className="flex flex-col sm:flex-row items-center justify-between gap-4">
             <div className="text-center sm:text-left">
              <h1 className="text-3xl font-bold font-headline tracking-tight sm:text-4xl">
                Selamat Datang di AkselAI
              </h1>
              <p className="mt-2 max-w-2xl text-lg text-muted-foreground">
                {isTrialActive
                  ? 'Pilih, buat, atau kelola Partner AI Anda di bawah ini.'
                  : 'Masa uji coba gratis Anda telah berakhir. Terima kasih telah mencoba AkselAI.'}
              </p>
            </div>
            {isTrialActive && (
              <ClientOnly>
                <div className="flex items-center gap-2">
                  <Button variant="outline" size="sm" onClick={resetPartners}>
                    <RotateCcw className="mr-2 h-4 w-4" />
                    Reset
                  </Button>
                  <Button size="sm" onClick={() => setCreateDialogOpen(true)}>
                    <PlusCircle className="mr-2 h-4 w-4" />
                    Buat Partner Baru
                  </Button>
                </div>
              </ClientOnly>
            )}
          </div>
        </div>

        <ClientOnly>
          <div className="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4">
            {partners.map(partner => (
              <PartnerCard
                key={partner.slug}
                partner={partner}
                onDelete={() => deletePartner(partner.slug)}
              />
            ))}
          </div>
          <div className="mt-8 pt-8 border-t">
             <StrategicAdvisorCard />
          </div>
          {isTrialActive && partners.length < 8 && (
              <div className="mt-8 md:col-span-2 lg:col-span-1 xl:col-span-4">
                <FeedbackCard />
              </div>
            )}
        </ClientOnly>
      </div>
      <CreatePartnerDialog
        isOpen={isCreateDialogOpen}
        onOpenChange={setCreateDialogOpen}
        onPartnerCreated={addPartner}
      />
    </>
  );
}
```

---
### `src/lib/partners.ts`
```ts
import type { LucideIcon } from 'lucide-react';
import * as LucideIcons from 'lucide-react';

export type Partner = {
  slug: string;
  name: string;
  skill: string;
  description?: string;
  icon: keyof typeof LucideIcons;
  price: number;
  tier: 'Basic' | 'Pro' | 'Enterprise';
  version: number;
};

// These are the icons available for auto-selection for new partners.
const availableIcons: (keyof typeof LucideIcons)[] = [
  'Activity', 'Airplay', 'Album', 'Archive', 'Atom', 'Award', 'BadgeCheck',
  'Beaker', 'Bell', 'Book', 'Bookmark', 'BrainCircuit', 'Briefcase', 'Brush', 'Calculator',
  'Calendar', 'Camera', 'CircuitBoard', 'Clipboard', 'Cloud', 'Cog', 'Compass',
  'Computer', 'Copy', 'Crown', 'Database', 'Diamond', 'DraftingCompass', 'ShieldCheck',
  'Edit', 'Feather', 'Film', 'Filter', 'Flag', 'FlaskConical', 'Folder',
  'Gem', 'Gift', 'GraduationCap', 'Heart', 'Home', 'Image', 'Inbox', 'Key',
  'Landmark', 'Languages', 'Layers', 'LayoutGrid', 'Library', 'LifeBuoy', 'Lightbulb',
  'Link', 'Lock', 'Mail', 'Map', 'Medal', 'Megaphone', 'MessageSquare',
  'Mic', 'Moon', 'MousePointer', 'Music', 'Newspaper', 'Nut', 'Package',
  'Paintbrush', 'Palette', 'Paperclip', 'Pen', 'Percent', 'Phone', 'PieChart',
  'Pin', 'Plane', 'Puzzle', 'Quote', 'Receipt', 'Rocket', 'Ruler', 'Save',
  'Scale', 'Scissors', 'ScreenShare', 'Send', 'Settings', 'Shield', 'ShoppingBag',
  'Smile', 'Sparkles', 'Speaker', 'Star', 'Sun', 'Sunrise', 'Sunset', 'Sword',
  'Table', 'Tag', 'Target', 'Tent', 'Terminal', 'ThumbsUp', 'Ticket', 'Timer',
  'ToggleLeft', 'Tool', 'Train', 'Trash', 'TrendingUp', 'Trophy', 'Umbrella',
  'Users', 'Video', 'Wallet', 'Watch', 'Wind', 'Wrench', 'Zap', 'Code', 'Bug', 'BarChart3'
];

export const getRandomIcon = (): keyof typeof LucideIcons => {
    return availableIcons[Math.floor(Math.random() * availableIcons.length)];
}

export const defaultPartners: Partner[] = [
  {
    slug: 'analis-kebijakan-publik',
    name: 'Analis Kebijakan Publik',
    skill: 'Analisis Data & Laporan Pemerintah',
    description: 'Partner AI untuk menganalisis data publik, merangkum laporan kompleks, dan memberikan rekomendasi kebijakan berbasis bukti.',
    icon: 'Landmark',
    price: 49,
    tier: 'Enterprise',
    version: 1.0,
  },
  {
    slug: 'cerdas-keuangan',
    name: 'Cerdas Keuangan',
    skill: 'Literasi dan Perencanaan Keuangan Pribadi',
    description: 'Partner AI untuk membantu pengguna memahami produk keuangan, membuat anggaran, dan merencanakan tujuan finansial.',
    icon: 'Wallet',
    price: 19,
    tier: 'Basic',
    version: 1.0,
  },
  {
    slug: 'umkm-maju',
    name: 'UMKM Maju',
    skill: 'Solusi Bisnis dan Keuangan untuk UMKM',
    description: 'Membantu UMKM dengan analisis pasar, strategi penjualan, dan manajemen keuangan sederhana untuk naik kelas.',
    icon: 'Briefcase',
    price: 29,
    tier: 'Pro',
    version: 1.0,
  },
   {
    slug: 'block-guardian',
    name: 'BlockGuardian',
    skill: 'Smart Contract Auditing & On-Chain Analysis',
    description: 'Membantu developer mengaudit smart contract untuk kerentanan umum dan menganalisis data on-chain untuk transparansi.',
    icon: 'ShieldCheck',
    price: 49,
    tier: 'Enterprise',
    version: 1.0,
  },
  {
    slug: 'code-companion',
    name: 'Code Companion',
    skill: 'Code Generation & Debugging',
    description: 'Your go-to partner for generating code snippets, debugging complex issues, and understanding programming concepts faster.',
    icon: 'Code',
    price: 29,
    tier: 'Pro',
    version: 1.0,
  },
  {
    slug: 'creative-writer',
    name: 'Creative Writer',
    skill: 'Content & Story Generation',
    description: 'Unleash your creativity with an AI that helps you write compelling stories, marketing copy, and engaging content.',
    icon: 'Pen',
    price: 19,
    tier: 'Basic',
    version: 1.0,
  },
  {
    slug: 'strategic-thinker',
    name: 'Strategic Thinker',
    skill: 'Business & Market Analysis',
    description: 'Get sharp insights and data-driven analysis to build robust business strategies and understand market trends.',
    icon: 'BrainCircuit',
    price: 49,
    tier: 'Enterprise',
    version: 1.0,
  },
  {
    slug: 'data-droid',
    name: 'Data Droid',
    skill: 'Data Analysis & Visualization',
    description: 'Transforms raw data into clear, actionable insights and beautiful visualizations to support your decisions.',
    icon: 'BarChart3',
    price: 49,
    tier: 'Enterprise',
    version: 1.0,
  },
];

export const getPartnerBySlug = (slug: string, partners: Partner[]): Partner | undefined => {
  return partners.find(partner => partner.slug === slug);
};
```

---
### `src/ai/flows/generate-pitch-ideas.ts`
```ts
'use server';

/**
 * @fileOverview A Genkit flow to generate strategic advice for a startup idea.
 *
 * It provides ideas for competitions to enter and key pitch points.
 * - generatePitchIdeas - The main function to call the flow.
 * - GeneratePitchIdeasInput - The input type for the flow.
 * - GeneratePitchIdeasOutput - The output type for the flow.
 */

import {ai} from '@/ai/genkit';
import {z} from 'genkit';

const GeneratePitchIdeasInputSchema = z.object({
  appName: z.string().describe('The name of the application.'),
  appDescription: z.string().describe('A brief description of what the application does.'),
  targetAudience: z.string().describe('The target audience for the application.'),
});
export type GeneratePitchIdeasInput = z.infer<typeof GeneratePitchIdeasInputSchema>;

const GeneratePitchIdeasOutputSchema = z.object({
  competitionSuggestions: z.array(z.object({
    category: z.string().describe('Kategori kompetisi (misalnya, Startup Umum, AI/ML, Dampak Sosial).'),
    justification: z.string().describe('Alasan mengapa kategori ini cocok untuk aplikasi tersebut.'),
  })).describe('Daftar saran kategori kompetisi.'),
  pitchPoints: z.array(z.object({
    point: z.string().describe('Poin penjualan utama untuk presentasi (pitch).'),
    elaboration: z.string().describe('Penjelasan singkat mengenai poin penjualan tersebut.'),
  })).describe('Poin-poin kunci untuk disertakan dalam pitch deck atau presentasi.'),
});
export type GeneratePitchIdeasOutput = z.infer<typeof GeneratePitchIdeasOutputSchema>;


export async function generatePitchIdeas(input: GeneratePitchIdeasInput): Promise<GeneratePitchIdeasOutput> {
  return generatePitchIdeasFlow(input);
}

const prompt = ai.definePrompt({
  name: 'generatePitchIdeasPrompt',
  input: {schema: GeneratePitchIdeasInputSchema},
  output: {schema: GeneratePitchIdeasOutputSchema},
  system: `Anda adalah seorang penasihat startup kelas dunia. Tugas Anda adalah memberikan saran strategis yang konkret dan dapat ditindaklanjuti untuk proyek perangkat lunak tahap awal dalam Bahasa Indonesia.
Berdasarkan nama aplikasi, deskripsi, dan target audiens yang diberikan, Anda akan:
1.  Menyarankan 3-4 kategori kompetisi atau hackathon yang berbeda yang bisa diikuti oleh proyek tersebut. Untuk masing-masing, berikan justifikasi singkat.
2.  Menghasilkan 3-4 poin presentasi (pitch) yang kuat yang menyoroti kekuatan dan potensi proyek. Untuk setiap poin, berikan elaborasi singkat.
Fokus pada kreativitas, potensi pasar, dan inovasi. Saran harus bersifat mendorong dan praktis. Seluruh output harus dalam Bahasa Indonesia.`,
  prompt: `
Nama Aplikasi: {{appName}}
Deskripsi: {{appDescription}}
Target Audiens: {{targetAudience}}

Harap hasilkan saran kompetisi dan poin-poin presentasi utama berdasarkan informasi ini dalam Bahasa Indonesia.
`,
});

const generatePitchIdeasFlow = ai.defineFlow(
  {
    name: 'generatePitchIdeasFlow',
    inputSchema: GeneratePitchIdeasInputSchema,
    outputSchema: GeneratePitchIdeasOutputSchema,
  },
  async input => {
    const {output} = await prompt(input);
    if (!output) {
      throw new Error('Failed to generate strategic advice.');
    }
    return output;
  }
);
```

... dan seterusnya untuk semua file penting lainnya.
