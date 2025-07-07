# Anatomica Fantastica: The Multispecies Medical Archive

A comprehensive medical encyclopedia for fantasy species, built with Jekyll and hosted on GitHub Pages.

## 🏥 About

Anatomica Fantastica is a scholarly archive documenting the medical treatment, physiology, and healing practices of fantasy species across the multiverse. From the iron allergies of elves to the robust constitution of dwarves, this encyclopedia serves as an essential reference for healers and medical practitioners in fantasy settings.

## 📚 Featured Species

Currently documented species include:
- **Humans** - Adaptable and magically variable
- **Elves** - Magically sensitive with iron allergies  
- **Dwarves** - Robust constitution and forge-related health concerns
- **Fae** - Immortal magical beings with reality-altering abilities
- **Dragons** - Ancient magical creatures with complex physiology
- **Orcs** - Warrior culture with enhanced combat physiology
- *(More species entries coming soon)*

## 🛠️ Built With

- **Jekyll** - Static site generator
- **GitHub Pages** - Hosting platform
- **Markdown** - Content format
- **Liquid** - Template language

## 🚀 Getting Started

### Prerequisites
- **Ruby** 2.7+ (for local development)
- **Jekyll** 4.3+
- **Bundler** gem
- **Git**
- **VS Code Extensions** (recommended):
  - Ruby LSP (Shopify.ruby-lsp) - Modern Ruby language support
  - Jekyll Snippets - For Jekyll-specific code completion

#### Installing Ruby and Jekyll on Windows:

1. Download and install Ruby from [RubyInstaller](https://rubyinstaller.org/)
2. Install Jekyll and Bundler:
   ```powershell
   gem install jekyll bundler
   ```

#### Installing on macOS:
```bash
brew install ruby
gem install jekyll bundler
```

#### Installing on Linux:
```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
gem install jekyll bundler
```

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fantasy-medical-encyclopedia.git
   cd fantasy-medical-encyclopedia
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Run the development server:
   ```bash
   bundle exec jekyll serve --livereload
   ```

4. Open your browser to `http://localhost:4000`

**VS Code Users:** Use the "Jekyll: Serve" task from the command palette (`Ctrl+Shift+P`) to start the development server with live reload.

### GitHub Pages Deployment

This site is configured for automatic deployment to GitHub Pages. Simply:

1. Push your changes to the `main` branch
2. GitHub Actions will automatically build and deploy the site
3. Your site will be available at `https://yourusername.github.io/fantasy-medical-encyclopedia`

## 📝 Adding Content

### Adding a New Species

1. Create a new Markdown file in the `_species/` directory
2. Use the following front matter template:
   ```yaml
   ---
   title: "Species Name"
   layout: species
   lifespan: "X-Y years"
   ---
   ```

3. Follow the established content structure with emoji headers:
   - 🧬 Lifespan
   - 📏 Physical Characteristics  
   - 🫀 Cardiovascular & Respiratory Systems
   - 🩺 Common Ailments & Vulnerabilities
   - ✨ Magical Anomalies / Biological Adaptations
   - 🧪 Healing Response
   - 🥼 Crossbreeding Compatibility
   - 🧂 Allergies / Magical Toxins
   - 🌿 Cultural Medical Practices
   - 📓 Scholar's Notes

### Content Guidelines

- Maintain a scholarly but engaging tone
- Include practical medical information (dosages, protocols, warnings)
- Balance fantasy elements with medical realism
- Add cross-references to other species when relevant
- Include cultural sensitivity in treatment approaches

## 🎨 Customization

### Styling
- Main styles are included in individual page headers
- The site uses Jekyll's default Minima theme as a base
- Responsive design with CSS Grid for species cards

### Configuration
- Edit `_config.yml` for site-wide settings
- Modify navigation in the config file
- Update site metadata and GitHub Pages URL

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-species`)
3. Commit your changes (`git commit -am 'Add new species entry'`)
4. Push to the branch (`git push origin feature/new-species`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- The Transcendental Medical College for research standards
- All the fictional healers and physicians who contributed their knowledge
- The multispecies communities who shared their medical traditions

---

*"Medicine is the great equalizer—disease and injury affect all species."*  
**—Archmedicus Theren Goldleaf**
