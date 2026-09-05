"# My Portfolio (Vite + React + TypeScript)" 

###
During Hosting i have encountered differernt issues 

  1.Firstly if you experience white screen issue then it's typically the static yml configuration issue during deployment,bcz the normal static website differs from vite+react app.
  SOLUTION : change the static yml file while hosting with npm hosting yml file.
  
 2.If you are new to vite+react project don't just download all files and host it,leave the ./github dir bcz it causes the white screen issue,create your own on settings -> pages -> github actions -> static yml -> copy npm.yml -> paste in static.yml -> Then work website works fine !
 
  3.I have error while downloading my resume ,the resume was not downloaded with a error indicating no file on site ,check the app.tsx file.
  Wrong Code 
               {/* Download Resume Button */}
  <a
    href="/resume.pdf"
    download
     className="px-6 py-3 bg-gradient-to-r from-blue-500 to-purple-500 text-white 
             rounded-lg hover:from-blue-600 hover:to-purple-600 
             transition-all duration-300 flex items-center gap-2 
             transform hover:scale-105 shadow-lg"
  >
    <FileCode className="w-5 h-5" />
    Download Resume
  </a>
  
  Correct Version
               {/* Download Resume Button */}
<a
  href="./resume (2).pdf"
  download="resume (2).pdf"
  className="px-6 py-3 bg-gradient-to-r from-blue-500 to-purple-500 text-white rounded-lg hover:from-blue-600 hover:to-purple-600 transition-all duration-300 flex items-center gap-2 transform hover:scale-105 shadow-lg"
>
  <FileCode className="w-5 h-5" />
  Download Resume
</a>
###
       
