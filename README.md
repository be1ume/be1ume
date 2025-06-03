# Pac-Man Eating Contributions Animation for GitHub README

Below is a fun animated SVG of Pac-Man "eating" GitHub style contribution blocks. You can copy and paste this entire snippet into your GitHub profile README.md file to showcase the effect.

```markdown
<!-- Pac-Man Contribution Graph Animation -->
<div align="center">
<svg width="520" height="110" viewBox="0 0 520 110" fill="none" xmlns="http://www.w3.org/2000/svg" >
  <!-- Contribution blocks -->
  <g id="blocks">
    <rect x="10"  y="10" width="30" height="30" fill="#0e4429"/>
    <rect x="50"  y="10" width="30" height="30" fill="#006d32"/>
    <rect x="90"  y="10" width="30" height="30" fill="#26a641"/>
    <rect x="130" y="10" width="30" height="30" fill="#39d353"/>
    <rect x="170" y="10" width="30" height="30" fill="#0e4429"/>
    <rect x="210" y="10" width="30" height="30" fill="#006d32"/>
    <rect x="250" y="10" width="30" height="30" fill="#26a641"/>
    <rect x="290" y="10" width="30" height="30" fill="#39d353"/>
  
    <rect x="10"  y="50" width="30" height="30" fill="#006d32"/>
    <rect x="50"  y="50" width="30" height="30" fill="#26a641"/>
    <rect x="90"  y="50" width="30" height="30" fill="#39d353"/>
    <rect x="130" y="50" width="30" height="30" fill="#0e4429"/>
    <rect x="170" y="50" width="30" height="30" fill="#006d32"/>
    <rect x="210" y="50" width="30" height="30" fill="#26a641"/>
    <rect x="250" y="50" width="30" height="30" fill="#39d353"/>
    <rect x="290" y="50" width="30" height="30" fill="#0e4429"/>
  </g>

  <!-- Pac-Man -->
  <g id="pacman" transform="translate(10, 25)">
    <circle cx="15" cy="15" r="15" fill="#ffcc00" />
    <path id="mouth" fill="#1f1f1f" d="M15 15 L30 5 L30 25 Z">
      <animate 
        attributeName="d" 
        values="
          M15 15 L30 5 L30 25 Z;
          M15 15 L30 0 L30 30 Z;
          M15 15 L30 5 L30 25 Z
        " 
        dur="0.5s" 
        repeatCount="indefinite"
      />
    </path>
  </g>

  <!-- Animate Pac-Man moving across the blocks -->
  <animateTransform 
    xlink:href="#pacman" 
    attributeName="transform" 
    type="translate"
    values="10,25; 290,25; 10,25" 
    dur="6s" 
    repeatCount="indefinite"
  />
  
  <!-- Animate blocks being "eaten" -->
  <rect id="block-eaten-1" x="10" y="10" width="30" height="30" fill="#0e4429" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="0s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-2" x="50" y="10" width="30" height="30" fill="#006d32" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="0.75s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-3" x="90" y="10" width="30" height="30" fill="#26a641" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="1.5s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-4" x="130" y="10" width="30" height="30" fill="#39d353" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="2.25s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-5" x="170" y="10" width="30" height="30" fill="#0e4429" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="3s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-6" x="210" y="10" width="30" height="30" fill="#006d32" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="3.75s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-7" x="250" y="10" width="30" height="30" fill="#26a641" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="4.5s" repeatCount="indefinite"/>
  </rect>
  <rect id="block-eaten-8" x="290" y="10" width="30" height="30" fill="#39d353" opacity="1">
    <animate attributeName="opacity" values="1;0;1" dur="6s" begin="5.25s" repeatCount="indefinite"/>
  </rect>
</svg>
</div>
