<h1 align="center">✨ Alejo Capillera ✨</h1>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css">
    <title>Portafolio</title>
    <style>
        :root {
        --fondo : #fff;
        --fondo2: #F5F5F5;
        --fondo3: #ebeaea;
        --cielo : #5CE1E6;
        --cielo2 :#5ce1e641;
        --texto : #000000;
        --menu : rgba(255, 255, 255, 0.8);
        --linea:#DBDBDB;
        }
        .dark-mode {
        --fondo: #131313;
        --fondo2: #121212;
        --fondo3: #0c0c0c;
        --cielo: #34495e;
        --cielo2: #34495e94;
        --texto: #ecf0f1;
        --menu: #131313bb;
        --linea: #262626;
        }
/* Estilo del scroll */
::-webkit-scrollbar {
    width: 8px; /* Ancho del scroll */
}

::-webkit-scrollbar-track {
    background: var(--fondo); /* Fondo del scroll */
}

::-webkit-scrollbar-thumb {
    background-color: var(--fondo2); /* Color del scroll */
    border-radius: 10px; /* Bordes redondeados */
}

::-webkit-scrollbar-thumb:hover {
    background-color: var(--cielo); /* Color al pasar el mouse sobre el scroll */
}
        body{
            width:100%;
            height:100vh;
            margin:0;
            background-color: var(--fondo);
            font-family: Arial, sans-serif; /* Establece Arial como fuente principal */

        }
        .menu{
            display: flex; /* Usar flexbox para alinear elementos */
            width:100%;
            height:12%;
            background-color:var(--menu);
            position: fixed; 
            top: 0;
            left: 0; 
            z-index: 1000; 
            backdrop-filter: blur(10px);
            align-items: center; 
            justify-content: flex-end; /* Alinear a la derecha */

        }

        #toggle-mode{
            background-color:transparent;
            font-size:30px;
            color:var(--texto);
            border:0px solid;
            cursor:pointer;
            float:right;
            margin-right:1%;
        }

        .paisaje{
            position: relative;
            top: 12%; /* Coloca el SVG justo por debajo del menú */
            background-color:var(--cielo);
            width:100%;
            height:88%;
            transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */

        }

        svg{
            width:100%;
            height:100%;
            object-fit: cover;   /* Recorta el contenido como una imagen de fondo */
        }

    /* montañas */

    #svg_3 {
    animation: slideIn 1.5s forwards;
    }
    #svg_78 {
    animation: slideIn 1.8s forwards;
    }
    #svg_79 {
    animation: slideIn 1.5s forwards;
    }
    #svg_80 {
    animation: slideIn 1.8s forwards;
    }
    #svg_81 {
    animation: slideIn 1s forwards;
    }
    #svg_82 {
    animation: slideIn 1.5s forwards;
    }


    /* nubes*/
    #svg_87 {
    opacity: 1;
    animation: moveClouds 30s linear infinite 2s; 
    transform: translateX(-4000px); 
}
    #svg_90 {
    opacity: 1; 
    animation:moveClouds 35s linear infinite 2s; 
    transform: translateX(-4000px); 
}
    #svg_92 {
    opacity: 1; 
    animation:moveClouds 40s linear infinite 2s; 
    transform: translateX(-4000px);
}
    #svg_1 {
    opacity: 1;
    animation:moveClouds 45s linear infinite 2s;
    transform: translateX(-4000px);
    }

     /* ANIMACION MOVIMIENTO NUBES  */
    @keyframes moveClouds {
        0% {
            transform: translateX(-4000px); 
        }
        100% {
            transform: translateX(250vw); 
        }
        }

    /* sol */
    #svg_91{
        animation: slideIn 2.5s forwards;
    }

    #svg_91:hover {
        transform: scale(2); 
        cursor: pointer; 
        border:10px solid red;
    }

    #svg_55 {
        opacity:0;
    }
 /* ANIMACION APARICION */
@keyframes slideIn {
    from {
        transform: translateY(100%); 
    }
    to {
        transform: translateY(0);
    }
}


    .perfil{
        width:60%;
        height:100%;
        background-color: var(--fondo);
        margin-left:20%;
        margin-right:20%;
        transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */

        
    }
    .banner{
        width:100%;
        height:40%;
        background-color: var(--cielo);
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.10); /* Sombra solo en la parte inferior */
        transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */

    }
   .fotoperfil{
    background-color:var(--cielo);

        width:150px;
        height: 150px;
        margin-top:-10%;
        margin-left:3%;
        border-radius:100%;
        border:5px solid var(--fondo);
        cursor:pointer;
        box-shadow: 0 0 50px rgba(0, 0, 0, 0.2); /* Sombra más oscura y poco iluminada */
        transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */

    }
.descripcion{
    width:100%;
    height:30%;
}
h1{
    font-size:20px;
    color: var(--texto);
    margin-left:2%;
}
h2{
    font-size:14px;
    color: var(--texto);
    margin-left:2%;
}

    #dedo {
    transform: translateY(100%); /* Posición inicial fuera de la vista, desde abajo */
    transition: transform 0.5s ease; /* Animación de movimiento suave */
}

.fotoperfil:hover #dedo {
    transform: translateY(0); /* Mueve el elemento a su posición original */
}

.descripcion .button{
    background-color:var(--fondo3);
    width:20%;
    height:22%;
    border-radius:15px;
    border:0px solid;
    font-size:15px;
    font-weight: bold;
    cursor:pointer;
    float:right;
    margin-right:1%;
    margin-top:1%;
    color:var(--texto);
    transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */

}

.descripcion .button:hover {
    transform: scale(1.05); /* Aumenta el tamaño del botón al 110% */
}

.toggle-button {
width:50%;
height:10%;
float:left;
border:0px solid;
background-color: var(--fondo);
cursor:pointer;
transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */
color:var(--texto);
font-size:15px;
font-weight: bold;
}

.toggle-button:hover{
background-color: var(--cielo2);
}

.toggle-button.active {
    background-color: var(--cielo2);
    border-bottom:5px solid var(--cielo);
}

.boton{
    background-color:var(--fondo1);
    width:5%;
    height:22%;
    border:0px solid;
    font-size:15px;
    font-weight: bold;
    cursor:pointer;
    float:right;
    margin-right:1%;
    margin-top:1%;
    color:var(--texto);
    transition: background-color 0.3s ease, transform 0.4s ease; /* Transición suave para el color de fondo y el tamaño */

}

.boton:hover {
    transform: scale(1.1); /* Aumenta el tamaño del botón al 110% */
}

.content2{
    width:100%;
    height:200%;
    background-color:var(--fondo);
    transition: background-color 0.3s ease, transform 0.4s ease;
    padding-top:10%;

}



.post{
    width:90%;
    height:40%;
    margin-left:5%;
    margin-right:5%;
    border-radius:16px;
    border:1px solid var(--linea);
    margin-top:2%;
}
.arriba{
    display: flex; /* Activar Flexbox */
    width:100%;
    height:15%;
    align-items: center; /* Centrar horizontalmente */
    border-radius: 15px 15px 0 0;
    border-bottom:1px solid var(--linea);
}
.miniperfil{
    border-radius:100%;
    background-color: var(--cielo);
    margin-left:2%;
}
.abajo{
    width:100%;
    height:85%;
    border-radius: 0 0 15px 15px;
}

.imagen {
    width:90%;
    height:90%;
    margin-top:2%;
    margin-right:5%;
    margin-left:5%;
    margin-bottom:5%;
    border-radius:15px;

}
    @media (max-width: 1024px){
        .perfil{
        width:80%;
        margin-left:10%;
        margin-right:10%;
    }
    }
    @media (max-width: 600px) {
    .perfil{
        width:100%;
        margin-left:0%;
        margin-right:0%;
    }
    .banner{
        width:100%;
        height:35%;
    }
   .fotoperfil{
        width:120px;
        height: 120px;
        margin-top:-17%;
        margin-left:3%;
    }
    .descripcion .button{
    width:26%;
    height:22%;
    border-radius:15px;
    border:0px solid;
    font-size:15px;
    font-weight: bold;
    cursor:pointer;
    float:right;
    margin-right:1%;
    margin-top:1%;
}
.boton{
    margin-right:5%;

}

.post{
    width:100%;
    height:40%;
    margin-left:0%;
    margin-right:0%;
    border-radius:0px;
    border:0px solid var(--linea);
    margin-top:2%;
}
.arriba{
    display: flex; /* Activar Flexbox */
    width:100%;
    height:15%;
    align-items: center; /* Centrar horizontalmente */
    border-radius: 0px;
    border-bottom:1px solid var(--linea);
}

.abajo{
    width:100%;
    height:85%;
    border-radius: 05px;
}
    }
    </style>
</head>
<body>
    <div class="menu">
        <button id="toggle-mode"><i class="bi bi-moon-fill"></i></button>
    </div>
    <div class="paisaje">
        <svg viewBox="0 0 3460 1442" preserveAspectRatio="xMaxYMid slice" xmlns="http://www.w3.org/2000/svg">
            <g>
             <title>Layer 1</title>
             <path id="svg_12" d="m1327.6476,490.80444l0.745,-1.30375l0.745,1.30375l-1.49,0z" stroke-dasharray="2,2" stroke-width="0" stroke="#000" fill="#729C62"/>
             <path id="svg_20" d="m1387.52783,1112.57228l166.48071,-120.15467l-166.48071,120.15467z" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" stroke="#000" fill="#077a14"/>
             <path id="svg_37" d="m1378.36065,961.35619l-138.74169,52.07193" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" stroke="#000" fill="#052d60"/>
             <path id="svg_41" d="m435.3665,969.78976" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" stroke="#000" fill="#1b6821"/>
             <g stroke="null" id="svg_80">
              <path stroke="#000" id="svg_60" d="m1202.06455,1111.89565c375.37175,-592.53522 345.84814,-532.27741 342.4487,-533.29859c3.39944,1.02119 281.76501,508.19117 278.36557,507.16996" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c"/>
              <path stroke="#000" id="svg_68" d="m1545.34954,579.39145l278.09409,508.65151l-253.32088,14.4768" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
              <path stroke="#000" id="svg_76" d="m1543.70341,576.72688l-26.74578,43.17291l16.31712,-9.24703l10.88725,14.40245l4.83878,-17.28293l16.93572,7.20122" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded"/>
             </g>
             <g id="svg_78" stroke="null">
              <path id="svg_70" d="m2400.39702,988.52687l226.24811,-174.00018l132.87097,-41.53657l63.27189,80.10625l91.74424,148.3449l-94.90784,178.01388c1.53072,1.92011 -428.71816,-33.68267 -428.71816,-33.68267" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c" stroke="#000"/>
              <path id="svg_72" d="m2755.60635,777.0472l-76.74728,120.11182l90.43457,11.46106l-56.21609,263.60423l256.63862,13.75326l-70.24747,-252.48273" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141" stroke="#000"/>
             </g>
             <g stroke="null" id="svg_79">
              <path stroke="#000" id="svg_69" d="m1655.65253,1093.92143l478.07461,-629.48543l375.74975,620.20553" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c"/>
              <path stroke="#000" id="svg_71" d="m1880.1392,1094.23897l106.96005,-196.11l127.78779,61.28383c1.89622,2.83021 20.82775,-487.4405 20.82775,-487.4405c0,0 402.29491,631.69495 353.06986,633.57888" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
              <path stroke="#000" id="svg_77" d="m2133.46796,462.80095l-30.68257,42.08763l19.19454,-5.10686l9.46573,28.28475l9.46573,-27.10621l18.93145,7.33323" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded"/>
             </g>
             <g stroke="null" id="svg_81">
              <path stroke="#000" id="svg_62" d="m654.26372,1112.69642l326.27305,-346.6225l421.72008,286.88409l-241.97053,163.93375" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c"/>
              <path stroke="#000" id="svg_65" d="m980.97256,769.3606l309.72938,216.11375l-199.30815,194.10595" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
              <path stroke="#000" id="svg_75" d="m982.15775,765.17682l-36.05373,33.87353l23.24008,-2.81162l23.24008,14.05806l4.98001,-21.08709l26.56007,7.02903" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded"/>
             </g>
             <g stroke="null" id="svg_82">
              <path stroke="#000" id="svg_59" d="m-64.82749,964.02022c453.32332,-192.88398 449.23932,-187.93823 445.94762,-188.94402c3.29171,1.00579 231.99535,-271.01008 228.70366,-272.01586c3.29171,1.00579 305.50723,584.60345 302.21554,583.59765c3.29171,1.00579 -878.85097,149.37807 -882.14266,148.37228" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c"/>
              <path stroke="#000" id="svg_64" d="m666.87281,828.13908l-86.16705,-105.90382l-73.94535,171.30977l-109.31052,-50.61424l-414.73694,253.07126l45.01021,144.05595l630.14294,-101.22851" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
              <path stroke="#000" id="svg_67" d="m610.47794,504.17934l309.91345,589.87161l-259.24924,44.85036" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
              <path stroke="#000" id="svg_74" d="m611.46376,501.91305l-42.66523,49.51468l24.88792,-4.30563l21.3325,15.06973l8.88854,-17.22254l15.99939,12.91689l-28.44314,-55.97314l0.00002,0.00002z" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded"/>
             </g>
             <path stroke="#000" id="svg_91" d="m3157.85947,500.51367c-128.29635,0 -232.2164,-98.39172 -232.2164,-219.86298c0,-121.47126 103.92005,-219.86298 232.2164,-219.86298c128.29635,0 232.2164,98.39172 232.2164,219.86298c0,121.47126 -103.92005,219.86298 -232.2164,219.86298z" opacity="undefined" stroke-dasharray="2,2" stroke-width="0" fill="#E6C36A"/>
             <path id="svg_5" d="m2223.79029,1184.10131l71.04902,0.49731" opacity="NaN" stroke-width="0" stroke="#000" fill="#1b6821"/>
             <path id="svg_6" d="m2359.68581,1137.94812l604.3748,23.57391l261.53476,274.35509l-543.58205,17.94846l-266.66289,-92.30639l-174.35651,-28.20473" opacity="NaN" stroke-width="0" stroke="#000" fill="#1b6821"/>
             <g id="svg_13">
              <g stroke="null" id="svg_57">
               <g stroke="#000" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#1b6821" id="svg_52">
                <path stroke="#000" id="svg_45" d="m-70.23938,1239.57586c562.75567,-294.22506 2794.50588,-166.30112 2794.50588,-166.30112c0,0 3.8545,447.73378 3.03167,444.29022" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#1b6821"/>
                <path stroke="#000" id="svg_14" d="m-17.09845,1235.79359l2817.01691,0l0,237.64563l-2817.01691,0l0,-237.64563z" opacity="undefined" stroke-dasharray="2,2" stroke-width="0" fill="#07397c"/>
                <path stroke="#000" id="svg_39" d="m1397.11513,1238.71848l-264.97279,82.04539l144.17751,39.04173l1043.55024,7.7322" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#062f66"/>
                <path stroke="#000" id="svg_19" d="m1204.03015,1322.77295c859.46413,-367.35634 1176.87986,-178.27588 1176.55026,-178.48091c0.32959,0.20503 68.69607,200.09011 68.36646,199.88506" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#25822e"/>
                <path stroke="#000" id="svg_49" d="m2392.49014,1077.36907l419.3918,-28.95966l23.12519,375.21504l-589.69228,-81.01234" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#1b6821"/>
                <path stroke="#000" id="svg_51" d="m2512.60763,1337.46129l567.52057,0.79714l16.96443,260.56908l-822.77456,53.64657l-275.67189,-134.11643l254.46636,348.70275l-216.2964,-383.18983" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#25822e"/>
               </g>
               <path stroke="#000" id="svg_56" d="m426.92121,1158.47144c-558.88043,-319.79797 -558.88043,-319.79797 -555.79663,-323.20894c-3.0838,3.41096 -80.17075,412.75237 -77.08696,409.34141" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#1b6821"/>
              </g>
              <path id="svg_4" d="m2813.52556,1050.76986c0,0 787.16837,7.6922 786.42349,5.62545c0.74488,2.06675 -9.51138,391.80484 -10.25627,389.73807c0.74488,2.06677 -832.57669,14.8871 -833.32154,12.82033" opacity="NaN" stroke-width="0" stroke="#000" fill="#1b6821"/>
              <path stroke-dasharray="2,2" id="svg_9" d="m2326.35295,1132.81998l694.11712,21.00984l346.14895,312.81609l-782.04021,5.12813l-164.10024,-103.35882l-184.61277,-27.40856" opacity="NaN" stroke-width="0" stroke="#000" fill="#25822e"/>
             </g>
             <g stroke="null" id="svg_3">
              <g stroke="null" id="svg_34">
               <g stroke="null" id="svg_31">
                <path stroke="#000" id="svg_27" d="m2625.9409,1436.64637c362.10664,-717.61979 362.10664,-713.84283 361.83509,-713.98617c0.27157,0.14334 563.54856,230.53706 563.27699,230.39371c0.27159,0.14335 -72.14974,483.59246 -72.42133,483.44909c0.27157,0.14336 -1106.16538,192.76762 -1106.43692,192.62426" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c"/>
                <path stroke="#000" opacity="NaN" id="svg_28" d="m2903.82129,1153.00519l304.69948,130.27289l-96.53939,523.92984l-449.51154,-25.48848" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
                <path stroke="#000" opacity="NaN" id="svg_29" d="m2994.1127,1227.32949c-5.3635,-503.49466 -5.3635,-503.49466 -5.40912,-503.51877c0.04562,0.02411 303.08321,128.41524 303.03758,128.39114c0.04563,0.0241 -50.90759,453.16931 -50.95322,453.14519" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
                <path stroke="#000" id="svg_30" d="m2987.66476,724.08105l-55.09517,105.75892l37.9239,-15.10337c1.08234,1.0435 18.32048,28.01382 18.32048,28.01382c0,0 33.32706,-60.4135 32.24474,-61.45701c1.08233,1.04351 39.00623,15.06807 39.00623,15.06807c0,0 -2.29842,-29.12793 -3.38075,-30.17145c1.08233,1.04351 52.79675,6.43757 51.71441,5.39406" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded"/>
               </g>
               <path stroke="#000" id="svg_32" d="m2382.4281,1495.03033l16.08984,-98.1776l72.40436,-64.19304l120.67393,49.08879l64.35943,79.29729" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#424141"/>
               <path stroke="#000" id="svg_33" d="m2275.72776,1470.98314l52.29202,-71.74517l160.89857,71.74516" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#4c4c4c"/>
              </g>
              <path stroke="#000" stroke-dasharray="2,2" stroke-width="0" id="svg_35" d="m2931.32543,829.31466l56.34842,-110.06657l120.85647,49.91837c0.61577,0.65643 -103.30539,-19.17415 -103.30539,-19.17415" opacity="NaN" fill="#f2eded"/>
             </g>
             <g stroke="null" id="svg_55">
              <ellipse stroke="#000" ry="35.16894" rx="39.82491" id="svg_38" cy="271.4456" cx="3061.2739" stroke-dasharray="2,2" stroke-width="0" fill="#a38949"/>
              <ellipse stroke="#000" ry="35.16894" rx="39.82491" id="svg_44" cy="121.20355" cx="3173.90599" stroke-dasharray="2,2" stroke-width="0" fill="#a38949"/>
              <path stroke="#000" id="svg_46" d="m3325.24067,348.87618c-13.20163,0 -23.89495,-9.94016 -23.89495,-22.21196c0,-12.2718 10.69332,-22.21196 23.89495,-22.21196c13.20163,0 23.89495,9.94016 23.89495,22.21196c0,12.2718 -10.69332,22.21196 -23.89495,22.21196z" opacity="undefined" stroke-dasharray="2,2" stroke-width="0" fill="#a38949"/>
              <path stroke="#000" id="svg_53" d="m3050.44877,441.42603c-13.20164,0 -23.89496,-9.94016 -23.89496,-22.21196c0,-12.2718 10.69332,-22.21196 23.89496,-22.21196c13.20163,0 23.89494,9.94016 23.89494,22.21196c0,12.2718 -10.69332,22.21196 -23.89494,22.21196z" opacity="undefined" stroke-dasharray="2,2" stroke-width="0" fill="#a38949"/>
             </g>
             <g id="svg_1">
              <path id="svg_47" d="m2738.82091,367.69573l663.36687,-13.35431c-23.13037,-49.14972 -11.61337,-121.33854 -93.49362,-92.73124" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
              <path id="svg_48" d="m2757.81086,367.80918c27.88524,-25.2085 50.75104,-36.69726 78.6363,-61.9058l99.74932,22.03322c62.18527,-42.52296 110.31604,-24.28693 172.50131,-66.80989l118.13609,25.74264" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
             </g>
             <path id="svg_87" d="m1683.2514,274.03451l230.06966,-183.19121l101.1839,54.82959l202.36782,-65.7955l145.45186,115.14214l158.09986,-10.96593l69.56394,76.76142" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
             <path id="svg_90" d="m833.70971,493.89948c721.2487,-8.09401 711.80002,-4.04701 709.9095,-5.66643c1.89052,1.61942 -70.5493,-103.60259 -72.43982,-105.22199c1.89052,1.6194 -193.38205,58.27741 -195.27257,56.65799c1.89052,1.61942 -76.84843,-75.27358 -78.73893,-76.893c1.89051,1.61942 -139.83958,1.61942 -141.73009,0" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
             <g id="svg_92" stroke="null">
              <path id="svg_86" d="m319.03259,292.02714c728.06926,-11.91783 718.53124,-5.95893 716.62282,-8.34341c1.9084,2.38448 -71.21646,-152.54748 -73.12486,-154.93196c1.9084,2.38448 -195.21079,85.80938 -197.11918,83.42489c1.90838,2.38448 -77.57515,-110.83503 -79.48353,-113.21951c1.90838,2.38448 -141.16199,2.38448 -143.07037,0" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
              <path id="svg_88" d="m72.49552,296.34055l659.54984,-13.01704c-22.99727,-47.90844 -11.54653,-118.27413 -92.95566,-90.38931" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
              <path id="svg_89" d="m78.71106,296.67189c21.21233,-18.40902 38.60636,-26.79892 59.81871,-45.20797l75.8794,16.09021c47.30439,-31.05326 83.91751,-17.73602 131.22191,-48.78928l89.86624,18.79909" opacity="NaN" stroke-dasharray="2,2" stroke-width="0" fill="#f2eded" stroke="#000"/>
             </g>
            </g>
           
           </svg>    </div>
       
    
    
<script>

const toggleButton = document.getElementById('toggle-mode');
const body = document.body;
const svgElement = document.getElementById('svg_55'); // Selecciona el elemento SVG con id #svg_55

toggleButton.addEventListener('click', () => {
  // Alterna entre el modo oscuro y claro
  body.classList.toggle('dark-mode');

  // Cambia el texto y el ícono del botón dependiendo del modo
  if (body.classList.contains('dark-mode')) {
    toggleButton.innerHTML = '<i class="bi bi-sun-fill"></i>';
    svgElement.style.opacity = '1'; // Pone la opacidad a 1 en modo oscuro
  } else {
    toggleButton.innerHTML = '<i class="bi bi-moon-fill"></i>';
    svgElement.style.opacity = '0'; // Pone la opacidad a 0 en modo claro
  }
});


</script>

<script>
const buttons = document.querySelectorAll('.toggle-button');

buttons.forEach(button => {
    button.addEventListener('click', function() {
        // Eliminar la clase 'active' de todos los botones
        buttons.forEach(btn => btn.classList.remove('active'));
        
        // Agregar la clase 'active' solo al botón que fue presionado
        this.classList.add('active');
    });
});
</script>

</html>
