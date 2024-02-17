import Slider from "react-slick";
import "slick-carousel/slick/slick.css"; 
import "slick-carousel/slick/slick-theme.css";

import './App.css';

function App() {
  const settings = {
    dots: true,
    infinite: true,
    speed: 500,
    slidesToShow: 3,
    slidesToScroll: 1
  };
  return (
    <div className="App">
      <div className='parent'>
    <div className="child">
    <Slider {...settings}>
      {data.map((d) => (
        <div key={d.name} className="container">
          <div className='imgcon'>
            <img src={d.img} alt="" className="imge"/>
            
          </div>

          <div className="name">
            <p className="details">{d.name}</p>
            <a href="link" className="li">{d.link}</a>
            
          </div>
        </div>
        
      ))}
    </Slider>
    </div>
    </div>
    </div>
);
}
const data = [
  {
    name: `Ishita Raina`,
    img: `ishita.jpg`,
    link: "https://www.linkedin.com/in/ishitaraina1807/"
  },
  {
    name: `Rishabh Jain`,
    img: "rishab.jpg",
    link: `https://www.linkedin.com/in/rishabh-jain-69789622b/`
  },
  {
    name: `Himesh Parashar`,
    img: `himansh.jpg`,
    link: `https://www.linkedin.com/in/himeshparashar/`
  },
  {
    name: `Nandini Jinda`,
    img: `nand.jpg`,
    link: `https://www.linkedin.com/in/nandini-jindal-33a3a7282/`
  },
  {
    name: `Abdel Illah Belaoudj`,
    img: `abd.jpg`,
    link: `https://www.linkedin.com/in/abdelillahbel/`
  },
  {
    name: `Namya Jain`,
    img: `Namya .jpg`,
    link: `https://www.linkedin.com/in/namya-jain-bb9454215/`
  },
  
];



export default App;
