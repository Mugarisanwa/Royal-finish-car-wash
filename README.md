# Royal-finish-car-wash
Travel like royalty 👑
Royal Finish Car Wash
Services Pricing Gallery Contact Book Now
☰
Royal Finish Mobile Car Wash
Premium mobile washing & detailing in Harare. We come to you — home, office, anywhere.
Call 0778 751 478 Call 0784 873 025 See Pricing

Our Services
Exterior Wash
Hand wash, rinse, dry & tire shine for a spotless, streak-free finish.
Interior Detailing
Vacuum, wipe-down, dusting, windows & deodorize. Fresh cabin feel.
Waxing
Protective wax application for added shine and paint protection.
Premium Packages
Bundle interior + exterior + wax for the complete Royal Finish.
Simple Pricing
Small Vehicles
$20
Sedans, SUVs, Coupes, Hatchbacks
Book via WhatsApp
Big Vehicles
$40
Trucks, Freight, Buses
Book via WhatsApp
Need fleet or regular service? Contact us for custom quotes.
Before & After
See the Royal Finish difference. Replace these images with your own results.

Book Online
Name:
Vehicle Type:
            Sedan
            SUV
            Truck
            Bus
           Service:
            Exterior Wash
            Interior Detailing
            Waxing
            Premium Package
           Preferred Date/Time:
Notes:
Send to WhatsApp
Contact Us
Call Us
0778 751 478
0784 873 025
Social
Instagram: @royalfinishcarwash
Facebook: @royal_finish.zw
Service Area
We’re available across Harare.
© Royal Finish Car Wash. All rights reserved.
💬function toggleMenu(){
  const nav=document.querySelector('.nav');
  if(!nav) return;
  nav.style.display=(nav.style.display==='flex')?'none':'flex';
}
document.getElementById('year').textContent=new Date().getFullYear();

function isMobile(){
  return /Android|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent);
}

function sendToWhatsApp(event){
  event.preventDefault();
  let name=document.getElementById('name').value;
  let vehicle=document.getElementById('vehicle').value;
  let service=document.getElementById('service').value;
  let datetime=document.getElementById('datetime').value;
  let notes=document.getElementById('notes').value;
  let msg=`Hi, my name is ${name}. I’d like to book a ${service} for my ${vehicle} on ${datetime}. Notes: ${notes}`;
  let baseUrl=isMobile()? "https://wa.me/263778751478" : "https://web.whatsapp.com/send?phone=263778751478";
  let url=`${baseUrl}&text=${encodeURIComponent(msg)}`;
  window.open(url,'_blank');
}


function bookService(service, price){
  let msg=`Hi, I’d like to book a ${service} priced at ${price}.`;
  let baseUrl=isMobile()? "https://wa.me/263778751478" : "https://web.whatsapp.com/send?phone=263778751478";
  let url=`${baseUrl}&text=${encodeURIComponent(msg)}`;
  window.open(url,'_blank');
}
# Royal Finish Car Wash — Website (v2)

Features added:
- Booking form that redirects submissions to WhatsApp.
- Floating WhatsApp quick-chat button.
- Before/After gallery with placeholder images (replace with your own photos).
- Updated social media links.

To use:
1. Replace gallery placeholder images with your car wash before/after images in `assets/`.
2. Upload entire folder to hosting (Netlify, Vercel, cPanel, etc.).
3. Booking form will open WhatsApp with prefilled message using your number.
