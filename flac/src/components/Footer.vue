<template className="template">
  <footer className="footer">
    <div className="footer_top">
      <div className="container">
        <div className="footer_top-inner">
          <div className="footer_top-col1">
            
              <a className="footer_logo1" href="#">
                <img className="logo1" src="../assets/logo1.png" alt="logo1">
             </a>
            
          </div>
          <div className="footer_top-col2">
            
          
            <p>Product</p>
          
          
            <a className="footer_item-link" href="#">Features</a><br>
          
          
            <a className="footer_item-link" href="#">Integration</a><br>
          
          
            <a className="footer_item-link" href="#">Updates</a><br>
          
          
            <a className="footer_item-link" href="#">FAQ</a><br>
          
          
            <a className="footer_item-link" href="#">Pricing</a>
          
            
          </div>
          <div className="footer_top-col3">
            
            <p>Company</p>
          
          
            <a className="footer_item-link" href="#">About</a><br>
          
          
            <a className="footer_item-link" href="#">Blog</a><br>
        
          
            <a className="footer_item-link" href="#">Careers</a><br>
          
          
             <a className="footer_item-link" href="#">Manifesto</a><br>
          
             <a className="footer_item-link" href="#">Press</a><br>
          
          
             <a className="footer_item-link" href="#">Contract</a>
         
          </div>
          <div className="footer_top-col4">
            
            <p>Resources</p>
          
            <a className="footer_item-link" href="#">Examples</a><br>
          
            <a className="footer_item-link" href="#">Community</a><br>
          
            <a className="footer_item-link" href="#">Guides</a><br>
          
             <a className="footer_item-link" href="#">Docs</a><br>
          
             <a className="footer_item-link" href="#">Press</a>
          
          </div>
          <div className="footer_top-col5">
            
            <p>Legal</p>
          
            <a className="footer_item-link" href="#">Privacy</a><br>
          
            <a className="footer_item-link" href="#">Terms</a><br>  
          
            <a className="footer_item-link" href="#">Security</a>
          
          </div>
        </div>
      </div>
    </div>
    <div className="footer_bottom">
      
        <div className="footer_bottom-inner">
          
          <a className="footer_socials-link_x" href="#">
            <img className="link-x" src="../assets/vector_97_x2.svg" alt="vector_97">
          </a>
        
      
          <a className="footer_socials-link_insta" href="#">
             <img className="link-insta" src="../assets/vector_79_x2.svg" alt="vector_79">
          </a>
        
      
          <a className="footer_socials-link_youtube" href="#">
            <img className="link-youtube" src="../assets/vector_185_x2.svg" alt="vector_185">
          </a>
                          
        </div>
      
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent',
};
</script>

<style scoped>

.footer {
  color: #fff;
}
.footer_top {
  padding: 41px 0 0 
}

.footer_top {
  background-color: #020103;
}

.footer_top-list {
  list-style: none;
}

.footer_socials {
  list-style-type:  none;
}

.footer_top-inner {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  text-align: left;
  }

.footer_top-col1 {
  flex-grow: 5;
  padding-left: 45px;
}

.footer_top-col2 {
  flex-grow: 1;
}

.footer_top-col3 {
  flex-grow: 1;
}

.footer_top-col4 {
  flex-grow: 1;
}

.footer_top-col5 {
  flex-grow: 1;
}

.footer_item-link {
  text-decoration: none;
  color: #fff;
  opacity: 0.4;
  font-family: Inter;
  font-size: 13px;
  font-weight: 400;
  line-height: 26px;
  letter-spacing: -0.0001em;
  text-align: left;
  transition: 1ms;
}

.footer_item-link:hover {
  opacity: 1;
} 

.logo1 {
  width: 138px;
  height: 38px;
  border: 1px;
  box-shadow: 0px 4px 4px 0px #00000040;
}
 .footer_bottom {
  background-color: #020103;
  height: 65px;
}

.footer_bottom-inner {
  display: flex;
  flex-direction: row;
  padding-left: 45px;
}

.link-x {
  width: 24px;
  height: 24px;
  opacity: 0.4;
  padding-right: 15px;
  transition: 1ms;
}

.link-x:hover {
  opacity: 1;
}

.link-insta {
  width: 24px;
  height: 24px;
  opacity: 0.4;
  padding-left: 15px;
  padding-right: 15px;
  transition: 1ms;
}

.link-insta:hover {
  opacity: 1;
}

.link-youtube {
  width: 24px;
  height: 24px;
  opacity: 0.4;
  padding-left: 15px;
  transition: 1ms;
}

.link-youtube:hover {
  opacity: 1;
}
</style>
