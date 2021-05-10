1. Hello, my name is **Dmitry Pehterev**.
2. My cellphone 292817482 _(plus viber, telegram, WhatsApp account on this number)_, e-mail kelgreem@mail.ru.
3. I want to learn and improve in the kotlin lang, which was in the tone of my brain, and also implement my ideas on Android.
4. Now I know the basics: Pascal and Delphi, c++, c#, java, HTML, JS.
5. 

    //(JS code)  
    
    // this function will animate the virtual pendulum when it is hit by a bullet

    function animation(args) { 

	var $ = {
		radius  :     250 
	}
    
    krug=false;
	f = 0;
	s = 2 * Math.PI / 180; 
            
            
           var p1 = document.getElementById('u0_pul');
           
    var u0_a = p1.value;
    u0_a = Number(u0_a);        
            var p2 = document.getElementById('m_pul');
    var  m_pul = p2.value;
    m_pul = Number(m_pul);
            var p3 = document.getElementById('M2_pul');
    var   M2_pul = p3.value;
    M2_pul = Number(M2_pul);
            var p4 = document.getElementById('l_pul');
    var   l_pul = p4.value;
    l_pul = Number(l_pul);
                     
    v0_min = ((M2_pul+m_pul)*Math.sqrt(4*g*l_pul))/m_pul;
                  
    v0_mayat_pul = (m_pul*u0_a)/(m_pul+M2_pul);  
    u0_mayat_pul = (1/v0_mayat_pul)*1000;
            
    h_max =  Math.pow(v0_mayat_pul, 2)/(2*g);
    
            
     if (h_max > l_pul*2)  {       
    
     krug=true;
  
     }  
            
     pul_for_p_3(h_max, v0_min, v0_mayat_pul, l_pul*2); 
                            
     
     let   setIntervalID;        
	 setIntervalID = setInterval(function() {  
       
		f += s; 
        rez_v_cel = f * (180/Math.PI);
        
         h_tek = 2*l_pul*Math.pow(Math.sin(f/2), 2);
         d_tek = Math.sqrt( Math.pow(l_pul, 2)-Math.pow(l_pul-h_tek, 2)  );         

         pul_for_p(h_tek, d_tek, rez_v_cel);
 
          document.getElementById("timg1").style.transform = "rotate(" + -rez_v_cel + "deg)";
         
		  elem.style.left =  235 + $.radius * Math.sin(f)  + 'px';
		  elem.style.top =   235 + $.radius * Math.cos(f) + 'px';   
             
          r3.style.left = 235 + $.radius * Math.sin(f)  + 'px';
          r3.style.top = 235 + $.radius * Math.cos(f) + 10 + 'px';
          document.getElementById("pul").style.transform = "rotate(" + -rez_v_cel + "deg)"; 
         
          r4.style.left = 235 + $.radius * Math.sin(f)  + 10 +'px';
          r4.style.top = 235 + $.radius * Math.cos(f) + 5+ 'px';
          document.getElementById("im_dot").style.transform = "rotate(" + -rez_v_cel + "deg)"; 
    
    ttt++;    
      if (krug == true) {
        if (ttt>179) {
       clearInterval(setIntervalID); 
       elem.style.left = 229;
       elem.style.top = 484.84;
            but1.disabled = false;
            but2.disabled = false;
            but3.disabled = false;
        } 
      }  else {
       if ( h_tek>=h_max) {

           
           (function() {

    if (0 < f) {


        f -= s;
        rez_v_cel = f * (180/Math.PI);
        
        
        document.getElementById("timg1").style.transform = "rotate(" + -rez_v_cel + "deg)";
        elem.style.left =  235 + $.radius * Math.sin(f) - 5  +'px';
		  elem.style.top =   235 + $.radius * Math.cos(f) +'px';   
             
          r3.style.left = 235 + $.radius * Math.sin(f) - 5 + 'px';
          r3.style.top = 235 + $.radius * Math.cos(f) + 10 + 'px';
          document.getElementById("pul").style.transform = "rotate(" + -rez_v_cel + "deg)";
        
        
        setTimeout(arguments.callee, u0_mayat_pul);

    } else {

          but1.disabled = false;
          but2.disabled = false;
          but3.disabled = false; 

    }
    })();
          clearInterval(setIntervalID);
        }     
                
      } 
            
	}, u0_mayat_pul)
                  
    }  

6. Nothing...
7. Nothing  too...
8. School, university. _(I understand that this is not enough)_