<svg width="900" height="350" viewBox="0 0 900 350" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#000000"/>
      <stop offset="50%" style="stop-color:#0a001a"/>
      <stop offset="100%" style="stop-color:#000000"/>
    </linearGradient>

    <!-- Neon glow filter - MAGENTA -->
    <filter id="glowM" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="4" result="blur1"/>
      <feGaussianBlur stdDeviation="10" result="blur2"/>
      <feMerge>
        <feMergeNode in="blur2"/>
        <feMergeNode in="blur1"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Neon glow filter - CYAN -->
    <filter id="glowC" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="5" result="blur1"/>
      <feGaussianBlur in="blur1" stdDeviation="12" result="blur2"/>
      <feMerge>
        <feMergeNode in="blur2"/>
        <feMergeNode in="blur1"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Strong outer glow -->
    <filter id="glowStrong" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="8" result="b1"/>
      <feGaussianBlur stdDeviation="20" result="b2"/>
      <feGaussianBlur stdDeviation="35" result="b3"/>
      <feMerge>
        <feMergeNode in="b3"/>
        <feMergeNode in="b2"/>
        <feMergeNode in="b1"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Clip for scanlines -->
    <clipPath id="mainClip">
      <rect width="900" height="350"/>
    </clipPath>

    <!-- Glitch clip 1 -->
    <clipPath id="glitch1">
      <rect x="0" y="0" width="900" height="350"/>
    </clipPath>

    <!-- Mask for vignette -->
    <radialGradient id="vignette" cx="50%" cy="50%" r="70%">
      <stop offset="0%" style="stop-color:#000000;stop-opacity:0"/>
      <stop offset="100%" style="stop-color:#000000;stop-opacity:0.85"/>
    </radialGradient>
  </defs>

  <!-- BASE BACKGROUND -->
  <rect width="900" height="350" fill="url(#bgGrad)"/>

  <!-- ANIMATED GRID LINES - HORIZONTAL -->
  <g opacity="0.12" clip-path="url(#mainClip)">
    <line x1="0" y1="35" x2="900" y2="35" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="70" x2="900" y2="70" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="105" x2="900" y2="105" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="140" x2="900" y2="140" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="175" x2="900" y2="175" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="210" x2="900" y2="210" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="245" x2="900" y2="245" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="280" x2="900" y2="280" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="0" y1="315" x2="900" y2="315" stroke="#00ffff" stroke-width="0.5"/>
    <!-- VERTICAL -->
    <line x1="90" y1="0" x2="90" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="180" y1="0" x2="180" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="270" y1="0" x2="270" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="360" y1="0" x2="360" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="450" y1="0" x2="450" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="540" y1="0" x2="540" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="630" y1="0" x2="630" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="720" y1="0" x2="720" y2="350" stroke="#00ffff" stroke-width="0.5"/>
    <line x1="810" y1="0" x2="810" y2="350" stroke="#00ffff" stroke-width="0.5"/>
  </g>

  <!-- SCANLINES OVERLAY -->
  <g clip-path="url(#mainClip)" opacity="0.06">
    <rect x="0" y="0" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="3" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="6" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="9" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="12" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="15" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="18" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="21" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="24" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="27" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="30" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="33" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="36" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="39" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="42" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="45" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="48" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="51" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="54" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="57" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="60" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="63" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="66" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="69" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="72" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="75" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="78" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="81" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="84" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="87" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="90" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="93" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="96" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="99" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="102" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="105" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="108" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="111" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="114" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="117" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="120" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="123" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="126" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="129" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="132" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="135" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="138" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="141" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="144" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="147" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="150" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="153" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="156" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="159" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="162" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="165" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="168" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="171" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="174" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="177" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="180" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="183" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="186" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="189" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="192" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="195" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="198" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="201" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="204" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="207" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="210" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="213" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="216" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="219" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="222" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="225" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="228" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="231" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="234" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="237" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="240" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="243" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="246" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="249" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="252" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="255" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="258" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="261" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="264" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="267" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="270" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="273" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="276" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="279" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="282" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="285" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="288" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="291" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="294" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="297" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="300" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="303" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="306" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="309" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="312" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="315" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="318" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="321" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="324" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="327" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="330" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="333" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="336" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="339" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="342" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="345" width="900" height="1" fill="#ffffff"/>
    <rect x="0" y="348" width="900" height="1" fill="#ffffff"/>
  </g>

  <!-- CORNER BRACKETS -->
  <!-- Top-left -->
  <polyline points="15,45 15,15 55,15" fill="none" stroke="#ff00ff" stroke-width="2" filter="url(#glowM)">
    <animate attributeName="opacity" values="1;0.4;1;0.7;1" dur="3s" repeatCount="indefinite"/>
  </polyline>
  <!-- Top-right -->
  <polyline points="885,45 885,15 845,15" fill="none" stroke="#ff00ff" stroke-width="2" filter="url(#glowM)">
    <animate attributeName="opacity" values="1;0.4;1;0.7;1" dur="3s" begin="0.5s" repeatCount="indefinite"/>
  </polyline>
  <!-- Bottom-left -->
  <polyline points="15,305 15,335 55,335" fill="none" stroke="#00ffff" stroke-width="2" filter="url(#glowC)">
    <animate attributeName="opacity" values="1;0.3;1;0.8;1" dur="2.5s" begin="1s" repeatCount="indefinite"/>
  </polyline>
  <!-- Bottom-right -->
  <polyline points="885,305 885,335 845,335" fill="none" stroke="#00ffff" stroke-width="2" filter="url(#glowC)">
    <animate attributeName="opacity" values="1;0.3;1;0.8;1" dur="2.5s" begin="1.5s" repeatCount="indefinite"/>
  </polyline>

  <!-- DECORATIVE SIDE LINES -->
  <line x1="15" y1="60" x2="15" y2="120" stroke="#ff00ff" stroke-width="1" opacity="0.6" filter="url(#glowM)">
    <animate attributeName="y2" values="120;90;120" dur="2s" repeatCount="indefinite"/>
  </line>
  <line x1="885" y1="60" x2="885" y2="120" stroke="#ff00ff" stroke-width="1" opacity="0.6" filter="url(#glowM)">
    <animate attributeName="y2" values="120;90;120" dur="2s" begin="1s" repeatCount="indefinite"/>
  </line>
  <line x1="15" y1="230" x2="15" y2="290" stroke="#00ffff" stroke-width="1" opacity="0.6" filter="url(#glowC)">
    <animate attributeName="y1" values="230;260;230" dur="2s" begin="0.5s" repeatCount="indefinite"/>
  </line>
  <line x1="885" y1="230" x2="885" y2="290" stroke="#00ffff" stroke-width="1" opacity="0.6" filter="url(#glowC)">
    <animate attributeName="y1" values="230;260;230" dur="2s" begin="1.5s" repeatCount="indefinite"/>
  </line>

  <!-- HORIZONTAL ACCENT LINES TOP -->
  <rect x="0" y="0" width="900" height="2" fill="#ff00ff" opacity="0.7" filter="url(#glowM)">
    <animate attributeName="opacity" values="0.7;0.2;0.9;0.4;0.7" dur="4s" repeatCount="indefinite"/>
  </rect>
  <!-- HORIZONTAL ACCENT LINES BOTTOM -->
  <rect x="0" y="348" width="900" height="2" fill="#00ffff" opacity="0.7" filter="url(#glowC)">
    <animate attributeName="opacity" values="0.7;0.2;0.9;0.4;0.7" dur="4s" begin="2s" repeatCount="indefinite"/>
  </rect>

  <!-- GLITCH BLOCKS - random colored rectangles that flash -->
  <rect x="0" y="88" width="900" height="4" fill="#ff00ff" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0;0;0.6;0;0;0;0;0" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="y" values="88;88;88;88;88;88;155;88;88;88;88;88" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="height" values="4;4;4;4;4;4;2;4;4;4;4;4" dur="5s" repeatCount="indefinite"/>
  </rect>
  <rect x="50" y="140" width="800" height="3" fill="#00ffff" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0.5;0;0;0;0;0;0;0" dur="7s" begin="1s" repeatCount="indefinite"/>
    <animate attributeName="y" values="140;140;140;140;200;140;140;140;140;140;140;140" dur="7s" begin="1s" repeatCount="indefinite"/>
  </rect>
  <rect x="200" y="60" width="500" height="2" fill="#ffffff" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0;0;0;0.4;0;0;0;0;0;0" dur="9s" begin="2s" repeatCount="indefinite"/>
  </rect>

  <!-- ====== MAIN NAME - SHADOW LAYERS FOR DEPTH ====== -->

  <!-- Deep shadow layer -->
  <text x="454" y="170" font-family="'Arial Black', 'Impact', sans-serif" font-size="88" font-weight="900"
    text-anchor="middle" fill="#ff00ff" opacity="0.08" letter-spacing="8">ANIKET DALAL</text>

  <!-- CYAN OUTLINE - offset for 3D effect -->
  <text x="452" y="168" font-family="'Arial Black', 'Impact', sans-serif" font-size="88" font-weight="900"
    text-anchor="middle" fill="none" stroke="#00ffff" stroke-width="2" opacity="0.5" letter-spacing="8"
    filter="url(#glowC)">ANIKET DALAL</text>

  <!-- GLITCH LAYER 1 - shifts left occasionally -->
  <text x="454" y="170" font-family="'Arial Black', 'Impact', sans-serif" font-size="88" font-weight="900"
    text-anchor="middle" fill="#ff00ff" letter-spacing="8" filter="url(#glowM)" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0;0;0;1;0;0;0;0;0;0" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="x" values="454;454;454;454;454;454;454;440;454;454;454;454;454;454" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="y" values="170;170;170;170;170;170;170;172;170;170;170;170;170;170" dur="6s" repeatCount="indefinite"/>
    ANIKET DALAL
  </text>

  <!-- GLITCH LAYER 2 - shifts right occasionally -->
  <text x="454" y="170" font-family="'Arial Black', 'Impact', sans-serif" font-size="88" font-weight="900"
    text-anchor="middle" fill="#00ffff" letter-spacing="8" filter="url(#glowC)" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0;0;0;0;0;0;1;0;0;0" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="x" values="454;454;454;454;454;454;454;454;454;454;468;454;454;454" dur="8s" repeatCount="indefinite"/>
    ANIKET DALAL
  </text>

  <!-- MAIN NAME - PRIMARY WHITE with flicker -->
  <text x="454" y="170" font-family="'Arial Black', 'Impact', sans-serif" font-size="88" font-weight="900"
    text-anchor="middle" fill="#ffffff" letter-spacing="8" filter="url(#glowStrong)">
    <animate attributeName="opacity" values="1;1;1;1;1;1;0.95;1;1;1;0.85;1;1;0.92;1;1;1;1;0.97;1" dur="5s" repeatCount="indefinite"/>
    ANIKET DALAL
  </text>

  <!-- ANIMATED UNDERLINE -->
  <rect x="150" y="185" width="0" height="3" fill="#ff00ff" filter="url(#glowM)">
    <animate attributeName="width" values="0;600;600;600" dur="1.5s" fill="freeze"/>
    <animate attributeName="x" values="450;150;150;150" dur="1.5s" fill="freeze"/>
    <animate attributeName="opacity" values="1;1;0.6;1;0.8;1" dur="3s" begin="1.5s" repeatCount="indefinite"/>
  </rect>
  <rect x="150" y="190" width="0" height="1" fill="#00ffff" opacity="0.7" filter="url(#glowC)">
    <animate attributeName="width" values="0;600;600;600" dur="1.8s" fill="freeze"/>
    <animate attributeName="x" values="450;150;150;150" dur="1.8s" fill="freeze"/>
  </rect>

  <!-- SUBTITLE - FULL STACK DEVELOPER -->
  <text x="450" y="228" font-family="'Courier New', monospace" font-size="18" font-weight="700"
    text-anchor="middle" fill="#00ffff" letter-spacing="12" filter="url(#glowC)" opacity="0">
    <animate attributeName="opacity" values="0;0;0;1" dur="2s" fill="freeze"/>
    FULL-STACK DEVELOPER
  </text>

  <!-- DECORATIVE DOTS on subtitle -->
  <circle cx="175" cy="224" r="3" fill="#ff00ff" filter="url(#glowM)" opacity="0">
    <animate attributeName="opacity" values="0;0;0;1" dur="2.2s" fill="freeze"/>
    <animate attributeName="r" values="3;4;3;2;3" dur="2s" begin="2.2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="725" cy="224" r="3" fill="#ff00ff" filter="url(#glowM)" opacity="0">
    <animate attributeName="opacity" values="0;0;0;1" dur="2.2s" fill="freeze"/>
    <animate attributeName="r" values="3;4;3;2;3" dur="2s" begin="2.2s" repeatCount="indefinite"/>
  </circle>

  <!-- LOCATION TAG -->
  <text x="450" y="260" font-family="'Courier New', monospace" font-size="13"
    text-anchor="middle" fill="#ff6ec7" letter-spacing="5" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;1" dur="2.5s" fill="freeze"/>
    ◈  PUNE, INDIA  ◈  ONLINE  ◈  OPEN TO WORK  ◈
  </text>

  <!-- BOTTOM TECH STRIP -->
  <rect x="80" y="285" width="740" height="28" fill="#0a001a" rx="2" opacity="0.8"/>
  <rect x="80" y="285" width="740" height="28" fill="none" stroke="#ff00ff" stroke-width="0.5" rx="2" opacity="0.5"/>

  <text x="450" y="303" font-family="'Courier New', monospace" font-size="11"
    text-anchor="middle" fill="#ff00ff" letter-spacing="3" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0;1" dur="3s" fill="freeze"/>
    Java  ·  .NET  ·  Spring Boot  ·  React  ·  Node.js  ·  Docker  ·  Microservices
  </text>

  <!-- ANIMATED SCAN LINE that sweeps top to bottom -->
  <rect x="0" y="-10" width="900" height="6" fill="url(#scanGrad)" opacity="0.15">
    <animateTransform attributeName="transform" type="translate" values="0,0;0,360;0,0" dur="4s" repeatCount="indefinite"/>
  </rect>

  <!-- PULSING CORNER DOTS -->
  <circle cx="15" cy="15" r="4" fill="#ff00ff" filter="url(#glowM)">
    <animate attributeName="r" values="4;6;4;3;4" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.5;1;0.7;1" dur="2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="885" cy="15" r="4" fill="#ff00ff" filter="url(#glowM)">
    <animate attributeName="r" values="4;6;4;3;4" dur="2s" begin="0.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.5;1;0.7;1" dur="2s" begin="0.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="15" cy="335" r="4" fill="#00ffff" filter="url(#glowC)">
    <animate attributeName="r" values="4;6;4;3;4" dur="2s" begin="1s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.5;1;0.7;1" dur="2s" begin="1s" repeatCount="indefinite"/>
  </circle>
  <circle cx="885" cy="335" r="4" fill="#00ffff" filter="url(#glowC)">
    <animate attributeName="r" values="4;6;4;3;4" dur="2s" begin="1.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.5;1;0.7;1" dur="2s" begin="1.5s" repeatCount="indefinite"/>
  </circle>

  <!-- VIGNETTE OVERLAY -->
  <rect width="900" height="350" fill="url(#vignette)"/>

  <!-- RANDOM MATRIX CHARS - LEFT SIDE -->
  <text x="35" y="80" font-family="monospace" font-size="10" fill="#00ffff" opacity="0.3">01101</text>
  <text x="35" y="95" font-family="monospace" font-size="10" fill="#ff00ff" opacity="0.2">10010</text>
  <text x="35" y="110" font-family="monospace" font-size="10" fill="#00ffff" opacity="0.3">11001</text>
  <text x="35" y="125" font-family="monospace" font-size="10" fill="#ff00ff" opacity="0.15">01110</text>
  <text x="35" y="140" font-family="monospace" font-size="10" fill="#00ffff" opacity="0.25">10101</text>
  <!-- RIGHT SIDE -->
  <text x="830" y="80" font-family="monospace" font-size="10" fill="#ff00ff" opacity="0.3">11010</text>
  <text x="830" y="95" font-family="monospace" font-size="10" fill="#00ffff" opacity="0.2">01001</text>
  <text x="830" y="110" font-family="monospace" font-size="10" fill="#ff00ff" opacity="0.3">10110</text>
  <text x="830" y="125" font-family="monospace" font-size="10" fill="#00ffff" opacity="0.15">11100</text>
  <text x="830" y="140" font-family="monospace" font-size="10" fill="#ff00ff" opacity="0.25">01011</text>

  <!-- Flickering binary left with animation -->
  <g opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0.4;0;0;0;0;0.3;0;0" dur="7s" repeatCount="indefinite"/>
    <text x="35" y="160" font-family="monospace" font-size="10" fill="#00ffff">00111</text>
    <text x="35" y="175" font-family="monospace" font-size="10" fill="#ff00ff">10001</text>
    <text x="830" y="160" font-family="monospace" font-size="10" fill="#ff00ff">01100</text>
    <text x="830" y="175" font-family="monospace" font-size="10" fill="#00ffff">11011</text>
  </g>
</svg>
