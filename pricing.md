---
layout: default
lang: de
permalink: /pricing/
title: "Preise - Solobooks"
---

<!-- Hero Section -->
<section class="bg-white py-12 md:py-16">
  <div class="max-w-7xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-4">
        {{ site.data.translations[page.lang].pricing_page.hero_title }}
      </h1>
      <p class="text-lg md:text-xl text-gray-600 mb-8 max-w-3xl mx-auto">
        {{ site.data.translations[page.lang].pricing_page.hero_subtitle }}
      </p>
      <a
        href="{{ site.data.translations[page.lang].links.sign_up }}"
        class="inline-flex items-center justify-center bg-indigo-600 text-white font-semibold px-8 py-4 rounded-lg hover:bg-indigo-700 transition text-lg"
      >
        {{ site.data.translations[page.lang].pricing_page.hero_cta }}
      </a>
    </div>

    <!-- Pricing Cards -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto mb-16">
      <!-- Starter Plan -->
      <div class="bg-white border-2 border-gray-200 rounded-2xl p-8 shadow-sm hover:shadow-md transition text-left flex flex-col">
        <div class="mb-6">
          <div class="flex items-center gap-3 mb-3">
            <div class="w-10 h-10 bg-yellow-100 rounded-lg flex items-center justify-center">
              <svg class="w-6 h-6 text-yellow-600" fill="currentColor" viewBox="0 0 20 20">
                <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/>
              </svg>
            </div>
            <h3 class="text-2xl font-bold text-gray-900">{{ site.data.translations[page.lang].pricing_page.plans.starter.name }}</h3>
          </div>
          <p class="text-sm text-gray-500 mb-4">
            {{ site.data.translations[page.lang].pricing_page.plans.starter.description }}
          </p>
          <p class="text-3xl font-extrabold text-gray-900">
            {{ site.data.translations[page.lang].pricing_page.plans.starter.price }}
          </p>
        </div>
        <ul class="space-y-3 text-gray-700 flex-grow mb-6">
          {% for feature in site.data.translations[page.lang].pricing_page.plans.starter.included_features %}
          <li class="flex items-start">
            <svg class="w-5 h-5 text-green-500 mr-2 flex-shrink-0 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            <span>{{ feature }}</span>
          </li>
          {% endfor %}
          {% for feature in site.data.translations[page.lang].pricing_page.plans.starter.excluded_features %}
          <li class="flex items-start">
            <svg class="w-5 h-5 text-red-500 mr-2 flex-shrink-0 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
            </svg>
            <span class="text-gray-400">{{ feature }}</span>
          </li>
          {% endfor %}
        </ul>
        <a
          href="{{ site.data.translations[page.lang].links.sign_up_starter }}"
          class="text-center bg-gray-100 text-gray-700 font-semibold px-6 py-3 rounded-lg hover:bg-gray-200 transition w-full mb-2"
        >
          {{ site.data.translations[page.lang].pricing_page.plans.starter.cta }}
        </a>
        <p class="text-xs text-gray-500 text-center">{{ site.data.translations[page.lang].pricing_page.plans.starter.cta_note }}</p>
      </div>

      <!-- Plus Plan -->
      <div class="bg-white border-2 border-gray-200 rounded-2xl p-8 shadow-sm hover:shadow-md transition text-left flex flex-col">
        <div class="mb-6">
          <div class="flex items-center gap-3 mb-3">
            <div class="w-10 h-10 bg-purple-100 rounded-lg flex items-center justify-center">
              <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/>
              </svg>
            </div>
            <h3 class="text-2xl font-bold text-gray-900">{{ site.data.translations[page.lang].pricing_page.plans.plus.name }}</h3>
          </div>
          <p class="text-sm text-gray-500 mb-4">
            {{ site.data.translations[page.lang].pricing_page.plans.plus.description }}
          </p>
          <p class="text-3xl font-extrabold text-gray-900">
            {{ site.data.translations[page.lang].pricing_page.plans.plus.price }}
            <span class="text-base font-normal text-gray-600">
              {{ site.data.translations[page.lang].pricing_page.plans.plus.period }}
            </span>
          </p>
        </div>
        <ul class="space-y-3 text-gray-700 flex-grow mb-6">
          {% for feature in site.data.translations[page.lang].pricing_page.plans.plus.included_features %}
          <li class="flex items-start">
            <svg class="w-5 h-5 text-green-500 mr-2 flex-shrink-0 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            <span>{{ feature }}</span>
          </li>
          {% endfor %}
          {% for feature in site.data.translations[page.lang].pricing_page.plans.plus.excluded_features %}
          <li class="flex items-start">
            <svg class="w-5 h-5 text-red-500 mr-2 flex-shrink-0 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
            </svg>
            <span class="text-gray-400">{{ feature }}</span>
          </li>
          {% endfor %}
        </ul>
        <a
          href="{{ site.data.translations[page.lang].links.sign_up_plus }}"
          class="text-center bg-gray-100 text-gray-700 font-semibold px-6 py-3 rounded-lg hover:bg-gray-200 transition w-full mb-2"
        >
          {{ site.data.translations[page.lang].pricing_page.plans.plus.cta }}
        </a>
        <p class="text-xs text-gray-500 text-center">{{ site.data.translations[page.lang].pricing_page.plans.plus.cta_note }}</p>
      </div>

      <!-- Pro Plan -->
      <div class="bg-gradient-to-br from-green-50 to-emerald-50 border-2 border-green-500 rounded-2xl p-8 shadow-lg relative text-left flex flex-col">
        <div class="absolute -top-4 right-6">
          <span class="bg-green-600 text-white text-xs font-semibold px-4 py-1 rounded-full">
            Beliebteste Wahl
          </span>
        </div>
        <div class="mb-6">
          <div class="flex items-center gap-3 mb-3">
            <div class="w-10 h-10 bg-green-100 rounded-lg flex items-center justify-center">
              <svg class="w-6 h-6 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/>
              </svg>
            </div>
            <h3 class="text-2xl font-bold text-gray-900">{{ site.data.translations[page.lang].pricing_page.plans.pro.name }}</h3>
          </div>
          <p class="text-sm text-gray-500 mb-4">
            {{ site.data.translations[page.lang].pricing_page.plans.pro.description }}
          </p>
          <p class="text-3xl font-extrabold text-gray-900">
            {{ site.data.translations[page.lang].pricing_page.plans.pro.price }}
            <span class="text-base font-normal text-gray-600">
              {{ site.data.translations[page.lang].pricing_page.plans.pro.period }}
            </span>
          </p>
        </div>
        <ul class="space-y-3 text-gray-700 flex-grow mb-6">
          {% for feature in site.data.translations[page.lang].pricing_page.plans.pro.included_features %}
          <li class="flex items-start">
            <svg class="w-5 h-5 text-green-500 mr-2 flex-shrink-0 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            <span>{{ feature }}</span>
          </li>
          {% endfor %}
        </ul>
        <a
          href="{{ site.data.translations[page.lang].links.sign_up_pro }}"
          class="text-center bg-green-600 text-white font-semibold px-6 py-3 rounded-lg hover:bg-green-700 transition w-full mb-2"
        >
          {{ site.data.translations[page.lang].pricing_page.plans.pro.cta }}
        </a>
        <p class="text-xs text-gray-500 text-center">{{ site.data.translations[page.lang].pricing_page.plans.pro.cta_note }}</p>
      </div>
    </div>

  </div>
</section>

<!-- Detailed Comparison Table -->
<section class="bg-gray-50 py-16 md:py-24">
  <div class="max-w-7xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ site.data.translations[page.lang].pricing_page.comparison_title }}
      </h2>
      <p class="text-lg text-gray-600">
        {{ site.data.translations[page.lang].pricing_page.comparison_subtitle }}
      </p>
    </div>

    <div class="bg-white rounded-xl shadow-lg overflow-hidden">
      <div class="overflow-x-auto">
        <table class="w-full">
          <thead>
            <tr class="bg-gray-50 border-b-2 border-gray-200">
              <th class="text-left py-4 px-6 font-semibold text-gray-900"></th>
              <th class="text-center py-4 px-6 font-semibold text-gray-900">
                <div class="flex flex-col items-center">
                  <span>{{ site.data.translations[page.lang].pricing_page.plans.starter.name }}</span>
                  <span class="text-sm font-normal text-gray-500">{{ site.data.translations[page.lang].pricing_page.plans.starter.price }}</span>
                </div>
              </th>
              <th class="text-center py-4 px-6 font-semibold text-gray-900">
                <div class="flex flex-col items-center">
                  <span>{{ site.data.translations[page.lang].pricing_page.plans.plus.name }}</span>
                  <span class="text-sm font-normal text-gray-500">{{ site.data.translations[page.lang].pricing_page.plans.plus.price }}{{ site.data.translations[page.lang].pricing_page.plans.plus.period }}</span>
                </div>
              </th>
              <th class="text-center py-4 px-6 font-semibold text-gray-900">
                <div class="flex flex-col items-center">
                  <span>{{ site.data.translations[page.lang].pricing_page.plans.pro.name }}</span>
                  <span class="text-sm font-normal text-gray-500">{{ site.data.translations[page.lang].pricing_page.plans.pro.price }}{{ site.data.translations[page.lang].pricing_page.plans.pro.period }}</span>
                </div>
              </th>
            </tr>
          </thead>
          <tbody>
            {% for category in site.data.translations[page.lang].pricing_page.comparison_categories %}
            <tr class="bg-indigo-50">
              <td colspan="4" class="py-3 px-6 font-bold text-gray-900">{{ category[1].name }}</td>
            </tr>
            {% for feature in category[1].features %}
            <tr class="border-b border-gray-200 hover:bg-gray-50">
              <td class="py-4 px-6 text-gray-700 font-medium">{{ feature.name }}</td>
              <td class="py-4 px-6 text-center">
                {% if feature.starter == true %}
                  <svg class="w-5 h-5 text-green-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                {% elsif feature.starter == false %}
                  <svg class="w-5 h-5 text-red-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                  </svg>
                {% else %}
                  <span class="text-gray-700">{{ feature.starter }}</span>
                {% endif %}
              </td>
              <td class="py-4 px-6 text-center">
                {% if feature.plus == true %}
                  <svg class="w-5 h-5 text-green-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                {% elsif feature.plus == false %}
                  <svg class="w-5 h-5 text-red-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                  </svg>
                {% else %}
                  <span class="text-purple-600 font-medium">{{ feature.plus }}</span>
                {% endif %}
              </td>
              <td class="py-4 px-6 text-center">
                {% if feature.pro == true %}
                  <svg class="w-5 h-5 text-green-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                {% elsif feature.pro == false %}
                  <svg class="w-5 h-5 text-red-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                  </svg>
                {% else %}
                  <span class="text-green-600 font-medium">{{ feature.pro }}</span>
                {% endif %}
              </td>
            </tr>
            {% endfor %}
            {% endfor %}
          </tbody>
        </table>
      </div>
    </div>

  </div>
</section>

<!-- FAQ Section -->
<section class="bg-white py-16 md:py-24">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ site.data.translations[page.lang].pricing_page.faq_title }}
      </h2>
    </div>

    <div class="space-y-4">
      {% for item in site.data.translations[page.lang].pricing_page.faq_items %}
      <div class="faq-item border border-gray-200 rounded-lg overflow-hidden">
        <button
          class="faq-question w-full text-left px-6 py-4 bg-gray-50 hover:bg-gray-100 transition flex items-center justify-between"
          onclick="toggleFaq({{ forloop.index0 }})"
        >
          <span class="font-semibold text-gray-900">{{ item.question }}</span>
          <svg
            class="faq-icon w-5 h-5 text-gray-500 transform transition-transform"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/>
          </svg>
        </button>
        <div
          class="faq-answer hidden px-6 py-4 bg-white text-gray-600"
          id="faq-answer-{{ forloop.index0 }}"
        >
          {{ item.answer }}
        </div>
      </div>
      {% endfor %}
    </div>

  </div>
</section>

<!-- Final CTA Section -->
<section class="bg-gradient-to-r from-indigo-600 to-indigo-800 py-20 md:py-32 text-center text-white">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <h2 class="text-3xl md:text-4xl font-bold mb-4">
      {{ site.data.translations[page.lang].final_cta.cta_title }}
    </h2>
    <p class="text-lg text-indigo-100 mb-8 max-w-2xl mx-auto">
      {{ site.data.translations[page.lang].final_cta.cta_description }}
    </p>
    
    <div class="flex flex-col sm:flex-row gap-4 justify-center mb-6">
      <a
        href="{{ site.data.translations[page.lang].links.sign_up }}"
        class="inline-flex items-center justify-center bg-white text-indigo-600 font-semibold px-8 py-4 rounded-lg hover:bg-indigo-50 transition"
      >
        {{ site.data.translations[page.lang].final_cta.cta_button }}
      </a>
      <a
        href="#"
        class="inline-flex items-center justify-center bg-indigo-600 text-white font-semibold px-8 py-4 rounded-lg hover:bg-indigo-700 transition border-2 border-indigo-500"
      >
        Demo ansehen
      </a>
    </div>

    <p class="text-sm text-indigo-200">
      Mehr als 5,000 deutsche Freelancer vertrauen bereits auf Solobooks
    </p>

  </div>
</section>

<script>
  function toggleFaq(index) {
    const button = event.currentTarget;
    const answer = document.getElementById('faq-answer-' + index);
    const icon = button.querySelector('.faq-icon');
    const isHidden = answer.classList.contains('hidden');
    
    // Close all other FAQs
    document.querySelectorAll('.faq-answer').forEach((el) => {
      el.classList.add('hidden');
    });
    document.querySelectorAll('.faq-icon').forEach((el) => {
      el.classList.remove('rotate-180');
    });
    
    // Toggle current FAQ
    if (isHidden) {
      answer.classList.remove('hidden');
      icon.classList.add('rotate-180');
    } else {
      answer.classList.add('hidden');
      icon.classList.remove('rotate-180');
    }
  }
</script>
