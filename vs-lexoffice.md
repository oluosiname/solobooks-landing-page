---
layout: default
lang: de
permalink: /vs/lexoffice/
title: "Günstige Lexoffice Alternative"
meta_description: "Suchen Sie eine günstige Lexoffice Alternative? Solobooks bietet Rechnungen, DATEV-Export & USt-VA ab €4,99/Monat. Jetzt kostenlos testen."
translations:
  en: /en/vs/lexoffice/
---

{% assign t = site.data.translations[page.lang].vs_lexoffice %}

<!-- Hero Section -->
<section class="bg-white py-16 md:py-24">
  <div class="max-w-4xl mx-auto px-4 md:px-12 text-center">
    <span class="inline-block bg-indigo-100 text-indigo-700 text-sm font-semibold px-4 py-1.5 rounded-full mb-6">
      {{ t.hero.badge }}
    </span>
    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6">
      {{ t.hero.title }}
      <span class="text-indigo-600">{{ t.hero.title_highlight }}</span>
    </h1>
    <p class="text-lg md:text-xl text-gray-600 mb-8 max-w-3xl mx-auto">
      {{ t.hero.subtitle }}
    </p>
    <div class="flex flex-col sm:flex-row gap-4 justify-center mb-6">
      <a
        href="{{ t.hero.cta_link }}"
        class="inline-flex items-center justify-center bg-indigo-600 text-white font-semibold px-8 py-4 rounded-lg hover:bg-indigo-700 transition text-lg"
      >
        {{ t.hero.cta_button }}
      </a>
      <a
        href="#comparison"
        class="inline-flex items-center justify-center bg-white text-gray-700 font-semibold px-8 py-4 rounded-lg hover:bg-gray-50 transition text-lg border-2 border-gray-200"
      >
        {{ t.hero.secondary_cta }}
      </a>
    </div>
    <p class="text-sm text-gray-500">{{ t.hero.trust_note }}</p>
  </div>
</section>

<!-- Feature Comparison Table -->
<section class="bg-gray-50 py-16 md:py-24" id="comparison">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ t.comparison_table.title }}
      </h2>
      <p class="text-lg text-gray-600">
        {{ t.comparison_table.subtitle }}
      </p>
    </div>

    <div class="bg-white rounded-xl shadow-lg overflow-hidden">
      <div class="overflow-x-auto">
        <table class="w-full">
          <thead>
            <tr class="bg-gray-50 border-b-2 border-gray-200">
              <th class="text-left py-4 px-6 font-semibold text-gray-900"></th>
              <th class="text-center py-4 px-6">
                <div class="flex flex-col items-center">
                  <span class="font-bold text-indigo-600 text-lg">{{ t.comparison_table.solobooks_label }}</span>
                </div>
              </th>
              <th class="text-center py-4 px-6">
                <div class="flex flex-col items-center">
                  <span class="font-bold text-gray-500 text-lg">{{ t.comparison_table.lexoffice_label }}</span>
                </div>
              </th>
            </tr>
          </thead>
          <tbody>
            {% for category in t.comparison_table.categories %}
            <tr class="bg-indigo-50">
              <td colspan="3" class="py-3 px-6 font-bold text-gray-900">{{ category[1].name }}</td>
            </tr>
            {% for feature in category[1].features %}
            <tr class="border-b border-gray-200 hover:bg-gray-50">
              <td class="py-4 px-6 text-gray-700 font-medium">{{ feature.name }}</td>
              <td class="py-4 px-6 text-center">
                {% if feature.solobooks == true %}
                  <svg class="w-5 h-5 text-green-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                {% elsif feature.solobooks == false %}
                  <svg class="w-5 h-5 text-red-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                  </svg>
                {% else %}
                  <span class="text-indigo-600 font-medium">{{ feature.solobooks }}</span>
                {% endif %}
              </td>
              <td class="py-4 px-6 text-center">
                {% if feature.lexoffice == true %}
                  <svg class="w-5 h-5 text-green-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                {% elsif feature.lexoffice == false %}
                  <svg class="w-5 h-5 text-red-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                  </svg>
                {% else %}
                  <span class="text-gray-700">{{ feature.lexoffice }}</span>
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

<!-- Pricing Comparison -->
<section class="bg-white py-16 md:py-24">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ t.pricing_comparison.title }}
      </h2>
      <p class="text-lg text-gray-600">
        {{ t.pricing_comparison.subtitle }}
      </p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-3xl mx-auto mb-10">
      <!-- Lexoffice Card -->
      <div class="bg-gray-50 border-2 border-gray-200 rounded-2xl p-8 text-center">
        <h3 class="text-xl font-bold text-gray-500 mb-4">{{ t.pricing_comparison.lexoffice_name }}</h3>
        <p class="text-4xl font-extrabold text-gray-400 mb-1">
          {{ t.pricing_comparison.lexoffice_price }}
          <span class="text-base font-normal text-gray-400">{{ t.pricing_comparison.lexoffice_period }}</span>
        </p>
        <p class="text-sm text-gray-400">{{ t.pricing_comparison.lexoffice_annual }}</p>
      </div>

      <!-- Solobooks Card -->
      <div class="bg-gradient-to-br from-green-50 to-emerald-50 border-2 border-green-500 rounded-2xl p-8 text-center relative">
        <h3 class="text-xl font-bold text-gray-900 mb-4">{{ t.pricing_comparison.solobooks_name }}</h3>
        <p class="text-4xl font-extrabold text-gray-900 mb-1">
          {{ t.pricing_comparison.solobooks_price }}
          <span class="text-base font-normal text-gray-600">{{ t.pricing_comparison.solobooks_period }}</span>
        </p>
        <p class="text-sm text-gray-600">{{ t.pricing_comparison.solobooks_annual }}</p>
      </div>
    </div>

    <!-- Savings Callout -->
    <div class="text-center mb-8">
      <div class="inline-flex items-center bg-green-100 text-green-800 font-bold text-lg px-6 py-3 rounded-full">
        {{ t.pricing_comparison.savings_text }}: {{ t.pricing_comparison.savings_amount }}
      </div>
    </div>

    <div class="text-center">
      <a
        href="{{ t.pricing_comparison.cta_link }}"
        class="inline-flex items-center justify-center bg-indigo-600 text-white font-semibold px-8 py-4 rounded-lg hover:bg-indigo-700 transition text-lg"
      >
        {{ t.pricing_comparison.cta_button }}
      </a>
    </div>
  </div>
</section>

<!-- Benefits Section -->
<section class="bg-indigo-50 py-16 md:py-24">
  <div class="max-w-6xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ t.benefits.title }}
      </h2>
      <p class="text-lg text-gray-600">
        {{ t.benefits.subtitle }}
      </p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      {% for benefit in t.benefits.items %}
      <div class="bg-white rounded-xl p-8 shadow-sm hover:shadow-md transition">
        <div class="w-12 h-12 bg-indigo-100 rounded-lg flex items-center justify-center mb-4">
          {% if benefit.icon == "currency" %}
          <svg class="w-6 h-6 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/>
          </svg>
          {% elsif benefit.icon == "export" %}
          <svg class="w-6 h-6 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4"/>
          </svg>
          {% elsif benefit.icon == "simple" %}
          <svg class="w-6 h-6 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/>
          </svg>
          {% elsif benefit.icon == "germany" %}
          <svg class="w-6 h-6 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/>
          </svg>
          {% endif %}
        </div>
        <h3 class="text-xl font-bold text-gray-900 mb-2">{{ benefit.title }}</h3>
        <p class="text-gray-600">{{ benefit.description }}</p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Testimonials -->
<section class="bg-gray-50 py-16 md:py-24">
  <div class="max-w-7xl mx-auto px-4 md:px-12">
    {% include testimonials.html %}
  </div>
</section>

<!-- FAQ Section -->
<section class="bg-white py-16 md:py-24">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ t.faq_title }}
      </h2>
    </div>

    <div class="space-y-4">
      {% for item in t.faq_items %}
      <div class="faq-item border border-gray-200 rounded-lg overflow-hidden">
        <button
          class="faq-question w-full text-left px-6 py-4 bg-gray-50 hover:bg-gray-100 transition flex items-center justify-between"
          onclick="toggleFaq({{ forloop.index0 }})"
        >
          <span class="font-semibold text-gray-900">{{ item.question }}</span>
          <svg
            class="faq-icon w-5 h-5 text-gray-500 transform transition-transform flex-shrink-0 ml-4"
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
      {{ t.final_cta.title }}
    </h2>
    <p class="text-lg text-indigo-100 mb-8 max-w-2xl mx-auto">
      {{ t.final_cta.subtitle }}
    </p>
    <a
      href="{{ t.final_cta.cta_link }}"
      class="inline-flex items-center justify-center bg-white text-indigo-600 font-semibold px-8 py-4 rounded-lg hover:bg-indigo-50 transition text-lg"
    >
      {{ t.final_cta.cta_button }}
    </a>
    <p class="text-sm text-indigo-200 mt-6">{{ t.final_cta.trust_note }}</p>
  </div>
</section>

<script>
  function toggleFaq(index) {
    const button = event.currentTarget;
    const answer = document.getElementById('faq-answer-' + index);
    const icon = button.querySelector('.faq-icon');
    const isHidden = answer.classList.contains('hidden');

    document.querySelectorAll('.faq-answer').forEach((el) => {
      el.classList.add('hidden');
    });
    document.querySelectorAll('.faq-icon').forEach((el) => {
      el.classList.remove('rotate-180');
    });

    if (isHidden) {
      answer.classList.remove('hidden');
      icon.classList.add('rotate-180');
    } else {
      answer.classList.add('hidden');
      icon.classList.remove('rotate-180');
    }
  }
</script>
