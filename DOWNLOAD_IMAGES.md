# Image Download Instructions

I couldn't download images from Wix's CDN due to network restrictions.
You need to save the following images to your `images/` folder before decommissioning your Wix site.

**Right-click → Save As** each image at the URLs below, using the filename shown:

| Save As | Source URL |
|---------|-----------|
| `images/naomi-hero.jpg` | https://static.wixstatic.com/media/79b7dd_80f74986babc4decaaf7ac8b92b28be0~mv2.jpg |
| `images/moonranger.jpg` | https://static.wixstatic.com/media/79b7dd_0c433329ccac4128aec8f215cab404e4~mv2.jpg |
| `images/mole-robot.jpg` | https://static.wixstatic.com/media/79b7dd_cd0feea88c24403d8f5530d4a7dc2077~mv2.jpg |
| `images/starlink.jpg` | https://static.wixstatic.com/media/79b7dd_97dc1b7e8b894a5292a2ef7b9ce5edf3~mv2.jpg |
| `images/irom-lab.png` | https://static.wixstatic.com/media/79b7dd_ec0e6803f9b94fc693b4df873af8de92~mv2.png |
| `images/mobility-aid.png` | https://static.wixstatic.com/media/79b7dd_764d2f6f3b7648ffac908493254efa32~mv2.png |
| `images/detonation-engine.png` | https://static.wixstatic.com/media/79b7dd_78ff3436f3a8408db20762f02de6f139~mv2.png |
| `images/mars-mission.jpg` | https://static.wixstatic.com/media/79b7dd_19504b73660941c5918e44bea5745673~mv2.jpg |
| `images/flying-fish.jpg` | https://static.wixstatic.com/media/79b7dd_6d2c083cea944093a19c27e9ffb03cfe~mv2.jpg |
| `images/rube-goldberg.png` | https://static.wixstatic.com/media/79b7dd_39ff1cf3d7274f6eb333c25ceac6f078~mv2.png |
| `images/airfoil-design.png` | https://static.wixstatic.com/media/79b7dd_9abf43e0a9be4e30937edc201a69326a~mv2.png |
| `images/hydrocar.jpg` | https://static.wixstatic.com/media/79b7dd_a1baa5378eed4977a2ca2ada7229d069~mv2.jpeg |
| `images/solar-cooker.png` | https://static.wixstatic.com/media/79b7dd_51eca812ec4449f6954c6a293c49fd76~mv2.png |
| `images/building-robot.jpg` | https://static.wixstatic.com/media/11062b_be6d973aaa1748aca87d52fbd1af37f0~mv2.jpg |

Or run this in your terminal:
```bash
cd images
curl -L "https://static.wixstatic.com/media/79b7dd_80f74986babc4decaaf7ac8b92b28be0~mv2.jpg" -o naomi-hero.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_0c433329ccac4128aec8f215cab404e4~mv2.jpg" -o moonranger.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_cd0feea88c24403d8f5530d4a7dc2077~mv2.jpg" -o mole-robot.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_97dc1b7e8b894a5292a2ef7b9ce5edf3~mv2.jpg" -o starlink.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_ec0e6803f9b94fc693b4df873af8de92~mv2.png" -o irom-lab.png
curl -L "https://static.wixstatic.com/media/79b7dd_764d2f6f3b7648ffac908493254efa32~mv2.png" -o mobility-aid.png
curl -L "https://static.wixstatic.com/media/79b7dd_78ff3436f3a8408db20762f02de6f139~mv2.png" -o detonation-engine.png
curl -L "https://static.wixstatic.com/media/79b7dd_19504b73660941c5918e44bea5745673~mv2.jpg" -o mars-mission.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_6d2c083cea944093a19c27e9ffb03cfe~mv2.jpg" -o flying-fish.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_39ff1cf3d7274f6eb333c25ceac6f078~mv2.png" -o rube-goldberg.png
curl -L "https://static.wixstatic.com/media/79b7dd_9abf43e0a9be4e30937edc201a69326a~mv2.png" -o airfoil-design.png
curl -L "https://static.wixstatic.com/media/79b7dd_a1baa5378eed4977a2ca2ada7229d069~mv2.jpeg" -o hydrocar.jpg
curl -L "https://static.wixstatic.com/media/79b7dd_51eca812ec4449f6954c6a293c49fd76~mv2.png" -o solar-cooker.png
curl -L "https://static.wixstatic.com/media/11062b_be6d973aaa1748aca87d52fbd1af37f0~mv2.jpg" -o building-robot.jpg
```

## GitHub Pages Custom Domain Setup

1. Push this repo to `github.com/YOUR_USERNAME/naomi-oke-web`
2. Go to Settings → Pages → Source: `main` branch
3. Under "Custom domain", enter `naomioke.me`
4. At your domain registrar, add these DNS records:
   - **A records** pointing to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **CNAME record**: `www` → `YOUR_USERNAME.github.io`
5. Check "Enforce HTTPS" in GitHub Pages settings
