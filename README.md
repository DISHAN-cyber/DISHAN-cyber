<img width="1180" height="610" alt="dark (1)" src="https://github.com/user-attachments/assets/1be770b3-a639-4952-a91c-a952ff9b4a50" />
<svg width="1180" height="610" viewBox="0 0 1180 610" xmlns="http://www.w3.org/2000/svg">
<defs>
  <linearGradient id="bgGrad" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#050814"/>
    <stop offset="100%" stop-color="#030712"/>
  </linearGradient>

  <radialGradient id="glowPurple" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#7C3AED" stop-opacity="0.35"/>
    <stop offset="100%" stop-color="#7C3AED" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="glowCyan" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity="0.30"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="glowEmerald" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#10B981" stop-opacity="0.22"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
  </radialGradient>

  <linearGradient id="accentGrad" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0%" stop-color="#7C3AED"/>
    <stop offset="50%" stop-color="#22D3EE"/>
    <stop offset="100%" stop-color="#10B981"/>
  </linearGradient>

  <linearGradient id="asciiGrad" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#A78BFA">
      <animate attributeName="stop-color" values="#A78BFA;#22D3EE;#10B981;#A78BFA" dur="6s" repeatCount="indefinite"/>
    </stop>
    <stop offset="50%" stop-color="#22D3EE">
      <animate attributeName="stop-color" values="#22D3EE;#10B981;#A78BFA;#22D3EE" dur="6s" repeatCount="indefinite"/>
    </stop>
    <stop offset="100%" stop-color="#10B981">
      <animate attributeName="stop-color" values="#10B981;#A78BFA;#22D3EE;#10B981" dur="6s" repeatCount="indefinite"/>
    </stop>
  </linearGradient>

  <linearGradient id="borderShimmer" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0%" stop-color="rgba(124,58,237,0)"/>
    <stop offset="50%" stop-color="rgba(124,58,237,0.9)"/>
    <stop offset="100%" stop-color="rgba(34,211,238,0)"/>
    <animateTransform attributeName="gradientTransform" type="translate" values="-2 0;2 0;-2 0" dur="5s" repeatCount="indefinite"/>
  </linearGradient>

  <filter id="softGlow" x="-60%" y="-60%" width="220%" height="220%">
    <feGaussianBlur stdDeviation="3.5" result="blur"/>
    <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>
  <filter id="bigBlur" x="-60%" y="-60%" width="220%" height="220%">
    <feGaussianBlur stdDeviation="30"/>
  </filter>
  <filter id="noiseFilter">
    <feTurbulence type="fractalNoise" baseFrequency="0.85" numOctaves="2" stitchTiles="stitch" result="noise"/>
    <feColorMatrix in="noise" type="matrix" values="0 0 0 0 1  0 0 0 0 1  0 0 0 0 1  0 0 0 0.025 0"/>
  </filter>

  <clipPath id="canvasClip"><rect x="0" y="0" width="1180" height="610" rx="28"/></clipPath>
  <clipPath id="leftClip"><rect x="24" y="24" width="430" height="562" rx="22"/></clipPath>
  <clipPath id="photoClip"><rect x="57" y="96" width="336" height="330" rx="20"/></clipPath>
  <clipPath id="photoRevealClip"><rect x="57" y="96" width="0" height="330"><animate attributeName="width" from="0" to="336" dur="1.3s" begin="0.2s" fill="freeze"/></rect></clipPath>

  <!-- typing clip paths: width animates 0 -> W -> W -> 0 within a 16s shared cycle -->
  <clipPath id="clipP0"><rect x="0" y="-16" width="0" height="24">
    <animate attributeName="width" dur="16s" repeatCount="indefinite"
      keyTimes="0;0.0875;0.1625;0.2;0.25;1" values="0;322;322;0;0;0"/>
  </rect></clipPath>
  <clipPath id="clipP1"><rect x="0" y="-16" width="0" height="24">
    <animate attributeName="width" dur="16s" repeatCount="indefinite"
      keyTimes="0;0.25;0.3375;0.4125;0.45;1" values="0;0;256;256;0;0"/>
  </rect></clipPath>
  <clipPath id="clipP2"><rect x="0" y="-16" width="0" height="24">
    <animate attributeName="width" dur="16s" repeatCount="indefinite"
      keyTimes="0;0.5;0.5875;0.6625;0.7;1" values="0;0;290;290;0;0"/>
  </rect></clipPath>
  <clipPath id="clipP3"><rect x="0" y="-16" width="0" height="24">
    <animate attributeName="width" dur="16s" repeatCount="indefinite"
      keyTimes="0;0.75;0.8375;0.9125;0.95;1" values="0;0;256;256;0;0"/>
  </rect></clipPath>
</defs>

<g clip-path="url(#canvasClip)">
<rect x="0" y="0" width="1180" height="610" fill="url(#bgGrad)"/>
<rect x="0" y="0" width="1180" height="610" filter="url(#noiseFilter)" opacity="0.5"/>

<circle cx="150" cy="120" r="160" fill="url(#glowPurple)" filter="url(#bigBlur)">
  <animate attributeName="cx" values="150;200;150" dur="14s" repeatCount="indefinite"/>
</circle>
<circle cx="1000" cy="500" r="200" fill="url(#glowCyan)" filter="url(#bigBlur)">
  <animate attributeName="cy" values="500;450;500" dur="16s" repeatCount="indefinite"/>
</circle>
<circle cx="900" cy="100" r="150" fill="url(#glowEmerald)" filter="url(#bigBlur)">
  <animate attributeName="cx" values="900;850;900" dur="12s" repeatCount="indefinite"/>
</circle>

<rect x="0" y="-40" width="1180" height="3" fill="#22D3EE" opacity="0.05">
  <animate attributeName="y" values="-40;650" dur="5s" repeatCount="indefinite"/>
</rect>

<g fill="#22D3EE">
  <circle cx="120" cy="500" r="2" opacity="0.6"><animate attributeName="cy" values="500;60;500" dur="9s" repeatCount="indefinite"/></circle>
  <circle cx="380" cy="480" r="1.6" opacity="0.5"><animate attributeName="cy" values="480;40;480" dur="11s" repeatCount="indefinite"/></circle>
  <circle cx="700" cy="550" r="2" opacity="0.5" fill="#7C3AED"><animate attributeName="cy" values="550;80;550" dur="10s" repeatCount="indefinite"/></circle>
  <circle cx="1050" cy="520" r="1.8" opacity="0.6" fill="#10B981"><animate attributeName="cy" values="520;60;520" dur="13s" repeatCount="indefinite"/></circle>
  <circle cx="850" cy="560" r="1.5" opacity="0.4"><animate attributeName="cy" values="560;100;560" dur="8s" repeatCount="indefinite"/></circle>
</g>

<!-- ============ LEFT PANEL ============ -->
<rect x="24" y="24" width="430" height="562" rx="22" fill="#0F172A" fill-opacity="0.6" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
<rect x="24" y="24" width="430" height="562" rx="22" fill="none" stroke="url(#borderShimmer)" stroke-width="1.4" opacity="0.9"/>

<g clip-path="url(#leftClip)">
  <path d="M24 24 L 300 24 L 100 586 L 24 586 Z" fill="#FFFFFF" opacity="0.02"/>

  <text x="50" y="65" font-family="Menlo, Consolas, monospace" font-size="12" fill="#94A3B8" letter-spacing="2">PROFILE.SYS</text>
  <circle cx="440" cy="60" r="4" fill="#10B981">
    <animate attributeName="opacity" values="1;0.3;1" dur="2s" repeatCount="indefinite"/>
  </circle>

  <g transform="translate(0,0)">
    <animateTransform attributeName="transform" type="translate" values="0,0;0,-6;0,0" dur="5s" repeatCount="indefinite" additive="sum"/>

   
  </g>

  <g font-family="Menlo, Consolas, monospace" opacity="0">
    <animate attributeName="opacity" to="1" begin="1.8s" dur="0.3s" fill="freeze"/>
    <text x="70" y="452" font-size="13" fill="url(#asciiGrad)">&lt; full-stack.dev /&gt;</text>
  </g>
  <rect x="70" y="464" width="9" height="16" fill="#22D3EE" opacity="0">
    <animate attributeName="opacity" begin="2.1s" values="0;1;1;0;0" keyTimes="0;0.1;0.5;0.6;1" dur="1s" repeatCount="indefinite"/>
  </rect>

  <g transform="translate(70,490)" font-family="Menlo, Consolas, monospace" font-size="13" opacity="0">
    <animate attributeName="opacity" to="1" begin="2.3s" dur="0.4s" fill="freeze"/>
    <text x="0" y="0" fill="#F8FAFC">📍 Sri Lanka</text>
    <text x="0" y="24" fill="#94A3B8">🎓 Undergraduate · Software Eng.</text>
    <text x="0" y="48" fill="#94A3B8">💼 Building @ Appitura</text>
  </g>

  <rect x="70" y="558" width="290" height="4" rx="2" fill="url(#accentGrad)" opacity="0">
    <animate attributeName="opacity" to="0.9" begin="2.6s" dur="0.4s" fill="freeze"/>
  </rect>
</g>

<!-- ============ RIGHT PANEL (terminal) ============ -->
<rect x="478" y="24" width="678" height="562" rx="22" fill="#0F172A" fill-opacity="0.6" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
<rect x="478" y="24" width="678" height="562" rx="22" fill="none" stroke="url(#borderShimmer)" stroke-width="1.4" opacity="0.9"/>

<rect x="478" y="24" width="678" height="42" rx="22" fill="#0B1220" fill-opacity="0.85"/>
<rect x="478" y="46" width="678" height="20" fill="#0B1220" fill-opacity="0.85"/>
<circle cx="504" cy="45" r="6" fill="#FF5F56"/>
<circle cx="524" cy="45" r="6" fill="#FFBD2E"/>
<circle cx="544" cy="45" r="6" fill="#27C93F"/>
<text x="817" y="50" text-anchor="middle" font-family="Menlo, Consolas, monospace" font-size="12" fill="#94A3B8">dishan@dev-terminal : ~</text>

<g font-family="Menlo, Consolas, 'Courier New', monospace">

  <text x="512" y="110" font-size="22" fill="#F8FAFC" opacity="0">Hi 👋
    <animate attributeName="opacity" to="1" begin="0.3s" dur="0.4s" fill="freeze"/>
  </text>
  <text x="512" y="148" font-size="28" font-weight="600" fill="url(#accentGrad)" opacity="0" filter="url(#softGlow)">I'm Dishan
    <animate attributeName="opacity" to="1" begin="0.8s" dur="0.5s" fill="freeze"/>
  </text>

  <!-- typing role phrases, cycling every 16s -->
  <g transform="translate(512,188)" opacity="0">
    <animate attributeName="opacity" to="1" begin="1.3s" dur="0.3s" fill="freeze"/>
    <text font-size="18" fill="#22D3EE">&gt;</text>
    <g transform="translate(20,0)" font-size="18" fill="#F8FAFC">
      <text clip-path="url(#clipP0)">Full-Stack Software Engineer</text>
      <text clip-path="url(#clipP1)">Java Backend Developer</text>
      <text clip-path="url(#clipP2)">React &amp; Flutter Developer</text>
      <text clip-path="url(#clipP3)">Open Source Enthusiast</text>
    </g>
    <rect y="-16" width="3" height="22" fill="#22D3EE">
      <animate attributeName="x" dur="16s" repeatCount="indefinite"
        keyTimes="0;0.0875;0.1625;0.2;0.25;0.3375;0.4125;0.45;0.5;0.5875;0.6625;0.7;0.75;0.8375;0.9125;0.95;1"
        values="20;342;342;20;20;276;276;20;20;310;310;20;20;276;276;20;20"/>
      <animate attributeName="opacity" values="1;0.15;1" dur="0.8s" repeatCount="indefinite"/>
    </rect>
  </g>

  <rect x="512" y="212" width="610" height="1" fill="rgba(255,255,255,0.08)"/>

  <g transform="translate(512,246)" font-size="13" opacity="0">
    <animate attributeName="opacity" to="1" begin="2s" dur="0.4s" fill="freeze"/>
    <text x="0" y="0" fill="#94A3B8">📍 Location</text><text x="120" y="0" fill="#F8FAFC">Sri Lanka</text>
    <text x="0" y="26" fill="#94A3B8">🎓 Education</text><text x="120" y="26" fill="#F8FAFC">Undergraduate, Software Eng.</text>
    <text x="0" y="52" fill="#94A3B8">💼 Focus</text><text x="120" y="52" fill="#F8FAFC">Full-Stack Engineer @ Appitura</text>
    <text x="0" y="78" fill="#94A3B8">🔗 LinkedIn</text><text x="120" y="78" fill="#F8FAFC">t-dishan-shayon</text>
  </g>

  <rect x="512" y="345" width="610" height="1" fill="rgba(255,255,255,0.08)"/>

  <text x="512" y="373" font-size="14" fill="#94A3B8" letter-spacing="1" opacity="0">
    ⚡ SKILLS &amp; TECH
    <animate attributeName="opacity" to="1" begin="2.4s" dur="0.4s" fill="freeze"/>
  </text>
</g>

<!-- skill pills -->
<g font-family="Menlo, Consolas, monospace" font-size="13">
  <!-- row 1 -->
  <g transform="translate(512,388)">
    <g opacity="0"><animate attributeName="opacity" to="1" begin="2.6s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(124,58,237,0.12)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">Java</text>
    </g>
    <g transform="translate(124,0)" opacity="0"><animate attributeName="opacity" to="1" begin="2.7s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(34,211,238,0.10)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="0.3s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">Spring Boot</text>
    </g>
    <g transform="translate(248,0)" opacity="0"><animate attributeName="opacity" to="1" begin="2.8s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(16,185,129,0.10)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="0.6s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">React</text>
    </g>
    <g transform="translate(372,0)" opacity="0"><animate attributeName="opacity" to="1" begin="2.9s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(124,58,237,0.12)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="0.9s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">TypeScript</text>
    </g>
    <g transform="translate(496,0)" opacity="0"><animate attributeName="opacity" to="1" begin="3.0s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(34,211,238,0.10)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="1.2s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">Node.js</text>
    </g>
  </g>
  <!-- row 2 -->
  <g transform="translate(512,430)">
    <g opacity="0"><animate attributeName="opacity" to="1" begin="3.1s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(16,185,129,0.10)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="1.5s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">Flutter</text>
    </g>
    <g transform="translate(124,0)" opacity="0"><animate attributeName="opacity" to="1" begin="3.2s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(124,58,237,0.12)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="1.8s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">PostgreSQL</text>
    </g>
    <g transform="translate(248,0)" opacity="0"><animate attributeName="opacity" to="1" begin="3.3s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(34,211,238,0.10)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="2.1s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">Docker</text>
    </g>
    <g transform="translate(372,0)" opacity="0"><animate attributeName="opacity" to="1" begin="3.4s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(16,185,129,0.10)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="2.4s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">AWS</text>
    </g>
    <g transform="translate(496,0)" opacity="0"><animate attributeName="opacity" to="1" begin="3.5s" dur="0.3s" fill="freeze"/>
      <rect width="114" height="32" rx="16" fill="rgba(124,58,237,0.12)" stroke="url(#accentGrad)" stroke-width="1" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="2.7s" repeatCount="indefinite"/>
      </rect>
      <text x="57" y="21" text-anchor="middle" fill="#F8FAFC">Git</text>
    </g>
  </g>
</g>

<rect x="512" y="490" width="610" height="1" fill="rgba(255,255,255,0.08)"/>

<!-- social icons -->
<g font-family="Menlo, Consolas, monospace" font-size="13" font-weight="600" opacity="0">
  <animate attributeName="opacity" to="1" begin="3.8s" dur="0.5s" fill="freeze"/>

  <g transform="translate(667,532)">
    <circle r="21" fill="rgba(255,255,255,0.04)" stroke="url(#accentGrad)" stroke-width="1.2" filter="url(#softGlow)">
      <animate attributeName="r" values="21;22.5;21" dur="3s" repeatCount="indefinite"/>
    </circle>
    <text text-anchor="middle" dy="5" fill="#F8FAFC" font-size="12">GH</text>
  </g>
  <g transform="translate(767,532)">
    <circle r="21" fill="rgba(255,255,255,0.04)" stroke="url(#accentGrad)" stroke-width="1.2" filter="url(#softGlow)">
      <animate attributeName="r" values="21;22.5;21" dur="3s" begin="0.4s" repeatCount="indefinite"/>
    </circle>
    <text text-anchor="middle" dy="5" fill="#F8FAFC" font-size="12">in</text>
  </g>
  <g transform="translate(867,532)">
    <circle r="21" fill="rgba(255,255,255,0.04)" stroke="url(#accentGrad)" stroke-width="1.2" filter="url(#softGlow)">
      <animate attributeName="r" values="21;22.5;21" dur="3s" begin="0.8s" repeatCount="indefinite"/>
    </circle>
    <text text-anchor="middle" dy="5" fill="#F8FAFC" font-size="12">X</text>
  </g>
  <g transform="translate(967,532)">
    <circle r="21" fill="rgba(255,255,255,0.04)" stroke="url(#accentGrad)" stroke-width="1.2" filter="url(#softGlow)">
      <animate attributeName="r" values="21;22.5;21" dur="3s" begin="1.2s" repeatCount="indefinite"/>
    </circle>
    <text text-anchor="middle" dy="5" fill="#F8FAFC" font-size="14">🌐</text>
  </g>
</g>

</g>
</svg>
