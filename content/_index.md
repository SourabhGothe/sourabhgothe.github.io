---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 Core Interests'
      subtitle: ''
      text: |-
        {{< rawhtml >}}
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 w-full max-w-none mt-4">
          <div>
            <h3 class="text-xl font-bold text-primary-600 dark:text-primary-400 mb-2">Research & Innovation</h3>
            <p class="italic text-gray-600 dark:text-gray-400 mb-6 text-sm">Exploring the boundaries of what AI can understand, reason, and generate.</p>
            
            <div class="mb-4 p-4 rounded-lg bg-gray-50 dark:bg-gray-800/50 border-l-4 border-primary-500 shadow-sm hover:shadow-md hover:-translate-y-0.5 transition-all duration-200">
              <div class="font-semibold text-gray-900 dark:text-white mb-1">Agentic Memory & Personalization</div>
              <div class="text-sm text-gray-600 dark:text-gray-400">RAG, GraphRAG, and lifelog intelligence on Knowledge Graphs for mobile ecosystems (AAAI 2026).</div>
            </div>

            <div class="mb-4 p-4 rounded-lg bg-gray-50 dark:bg-gray-800/50 border-l-4 border-primary-500 shadow-sm hover:shadow-md hover:-translate-y-0.5 transition-all duration-200">
              <div class="font-semibold text-gray-900 dark:text-white mb-1">Computer Vision & 3D Dynamics</div>
              <div class="text-sm text-gray-600 dark:text-gray-400">On-device physics engines, 2D to 3D dynamics (ICASSP 2025), and unsupervised event boundary detection (WACV 2024, ICASSP 2024).</div>
            </div>
            
            <div class="mb-4 p-4 rounded-lg bg-gray-50 dark:bg-gray-800/50 border-l-4 border-primary-500 shadow-sm hover:shadow-md hover:-translate-y-0.5 transition-all duration-200">
              <div class="font-semibold text-gray-900 dark:text-white mb-1">Generative AI & Multimodal NLP</div>
              <div class="text-sm text-gray-600 dark:text-gray-400">Large & Small Language Models (LLM/SLM) and semantic classification (CVIP 2022).</div>
            </div>
          </div>

          <div>
            <h3 class="text-xl font-bold text-primary-600 dark:text-primary-400 mb-2">Engineering & Productization</h3>
            <p class="italic text-gray-600 dark:text-gray-400 mb-6 text-sm">Optimizing and scaling AI to run flawlessly on millions of active devices.</p>
            
            <div class="mb-4 p-4 rounded-lg bg-gray-50 dark:bg-gray-800/50 border-l-4 border-primary-500 shadow-sm hover:shadow-md hover:-translate-y-0.5 transition-all duration-200">
              <div class="font-semibold text-gray-900 dark:text-white mb-1">On-Device Edge Inference</div>
              <div class="text-sm text-gray-600 dark:text-gray-400">Highly optimized network deployment, Quantization/Pruning, and LoRA adaptation for strict hardware constraints.</div>
            </div>

            <div class="mb-4 p-4 rounded-lg bg-gray-50 dark:bg-gray-800/50 border-l-4 border-primary-500 shadow-sm hover:shadow-md hover:-translate-y-0.5 transition-all duration-200">
              <div class="font-semibold text-gray-900 dark:text-white mb-1">Commercial Production Systems</div>
              <div class="text-sm text-gray-600 dark:text-gray-400">End-to-end commercialization of native C++ neural inference engines serving on Samsung Galaxy flagship devices (S24, S25, S26).</div>
            </div>

            <div class="mb-4 p-4 rounded-lg bg-gray-50 dark:bg-gray-800/50 border-l-4 border-primary-500 shadow-sm hover:shadow-md hover:-translate-y-0.5 transition-all duration-200">
              <div class="font-semibold text-gray-900 dark:text-white mb-1">Efficient Deep Learning Systems</div>
              <div class="text-sm text-gray-600 dark:text-gray-400">Architecting lightweight networks (e.g. 3M parameters) with SOTA accuracy.</div>
            </div>
          </div>
        </div>
        {{< /rawhtml >}}
    design:
      columns: '1'
      wide: true
  - block: collection
    id: papers
    content:
      title: Featured Publications
      count: 0
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: featured_patents
    content:
      title: Featured Patents
      count: 0
      filters:
        folders:
          - patents
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    id: patents
    content:
      title: Recent Patents
      text: ''
      filters:
        folders:
          - patents
        exclude_featured: false
    design:
      view: citation
  # News section disabled for now — re-enable once post images are corrected.
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     page_type: blog
  #     count: 10
  #     filters:
  #       author: ''
  #       category: ''
  #       tag: ''
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ''
  #     offset: 0
  #     order: desc
  #     view: card
  #     spacing:
  #       padding: [0, 0, 0, 0]
---
