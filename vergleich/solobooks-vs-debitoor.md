---
layout: default
lang: de
permalink: /vergleich/solobooks-vs-debitoor/
title: "Solobooks vs Debitoor – Die bessere Alternative für Freelancer"
translations:
  en: /en/compare/solobooks-vs-debitoor/
---

{% assign t = site.data.translations[page.lang].compare_debitoor %}

<!-- Hero Section -->
<section class="bg-gradient-to-br from-indigo-50 to-white py-16 md:py-24">
  <div class="max-w-5xl mx-auto px-4 md:px-12 text-center">
    <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">
      {{ t.hero_title }}
    </h1>
    <p class="text-lg md:text-xl text-gray-600 mb-8 max-w-3xl mx-auto">
      {{ t.hero_subtitle }}
    </p>
    <a
      href="{{ site.data.translations[page.lang].links.sign_up }}"
      class="inline-flex items-center justify-center bg-indigo-600 text-white font-semibold px-8 py-4 rounded-lg hover:bg-indigo-700 transition text-lg"
    >
      {{ t.hero_cta }}
    </a>
  </div>
</section>

<!-- Key Advantages -->
<section class="bg-white py-16 md:py-24">
  <div class="max-w-7xl mx-auto px-4 md:px-12">
    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 text-center mb-12">
      {{ t.advantages_title }}
    </h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {% for advantage in t.advantages %}
      <div class="bg-white border-2 border-gray-200 rounded-2xl p-8 shadow-sm hover:shadow-md transition text-center">
        <div class="w-14 h-14 bg-indigo-100 rounded-xl flex items-center justify-center mx-auto mb-6">
          {% if advantage.icon == "shield" %}
          <svg class="w-7 h-7 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/>
          </svg>
          {% elsif advantage.icon == "document" %}
          <svg class="w-7 h-7 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/>
          </svg>
          {% elsif advantage.icon == "export" %}
          <svg class="w-7 h-7 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-8l-4-4m0 0L8 8m4-4v12"/>
          </svg>
          {% endif %}
        </div>
        <h3 class="text-xl font-bold text-gray-900 mb-3">{{ advantage.title }}</h3>
        <p class="text-gray-600">{{ advantage.description }}</p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Feature Comparison Table -->
<section class="bg-gray-50 py-16 md:py-24">
  <div class="max-w-5xl mx-auto px-4 md:px-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
        {{ t.table_title }}
      </h2>
      <p class="text-lg text-gray-600">
        {{ t.table_subtitle }}
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
                  <span class="font-bold text-indigo-600 text-lg">{{ t.col_solobooks }}</span>
                </div>
              </th>
              <th class="text-center py-4 px-6">
                <div class="flex flex-col items-center">
                  <span class="font-semibold text-gray-500 text-lg">{{ t.col_debitoor }}</span>
                </div>
              </th>
            </tr>
          </thead>
          <tbody>
            {% for category in t.categories %}
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
                {% if feature.debitoor == true %}
                  <svg class="w-5 h-5 text-green-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                {% elsif feature.debitoor == false %}
                  <svg class="w-5 h-5 text-red-500 mx-auto" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                  </svg>
                {% else %}
                  <span class="text-gray-500">{{ feature.debitoor }}</span>
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

<!-- Why Freelancers Switch -->
<section class="bg-white py-16 md:py-24">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 text-center mb-10">
      {{ t.switch_title }}
    </h2>
    <ul class="space-y-4">
      {% for reason in t.switch_reasons %}
      <li class="flex items-start">
        <svg class="w-6 h-6 text-green-500 mr-3 flex-shrink-0 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
          <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
        </svg>
        <span class="text-lg text-gray-700">{{ reason }}</span>
      </li>
      {% endfor %}
    </ul>
  </div>
</section>

<!-- Testimonials -->
{% include testimonials.html %}

<!-- Final CTA Section -->
<section class="bg-gradient-to-r from-indigo-600 to-indigo-800 py-20 md:py-32 text-center text-white">
  <div class="max-w-4xl mx-auto px-4 md:px-12">
    <h2 class="text-3xl md:text-4xl font-bold mb-4">
      {{ site.data.translations[page.lang].final_cta.cta_title }}
    </h2>
    <p class="text-lg text-indigo-100 mb-8 max-w-2xl mx-auto">
      {{ site.data.translations[page.lang].final_cta.cta_description }}
    </p>
    <a
      href="{{ site.data.translations[page.lang].links.sign_up }}"
      class="inline-flex items-center justify-center bg-white text-indigo-600 font-semibold px-8 py-4 rounded-lg hover:bg-indigo-50 transition"
    >
      {{ site.data.translations[page.lang].final_cta.cta_button }}
    </a>
  </div>
</section>
