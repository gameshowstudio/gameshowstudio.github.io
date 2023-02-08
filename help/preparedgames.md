---
layout: help-page
title: Prepared Games
permalink: /help/preparedgames/
---

The host can prepare a game before getting everyone together to play, so that host can transition easily from one round to the next. Rounds in prepared games can have preplanned rules (e.g. scoring and timing rules) and question sets.

<table style="width: 100%">
    <colgroup>
        <col class="columnForTextInTableWithOtherColumnAsAnImage">
        <col>
    </colgroup>
    {% for element in site.data.updates.v3.preparedGamesConfig %}
    <tr>
        <td valign="top">
            {% if element.title %}<h4>{{ element.title }}</h4>{% endif %}
            {% for paragraph in element.paragraphs %}
                {{ paragraph }}
                <br>
                {% if element.image_importance == "high" %}
                <div class="hiddenOnLargeDevices">
                    <br>
                    <i>Click <a href="{{ element.image }}">here</a> for large image.</i><br><br>
                </div>
                {% endif %}
            {% endfor %}
        </td>
        {% if element.image_vertical_alignment %}<td valign="{{ element.image_vertical_alignment }}" align="right">{% else %}<td align="right">{% endif %}
            <a href="{{ element.image }}">
                <img src="{{ element.image }}" alt="{{ element.image_alt_text }}" width="98%">
            </a>
        </td>
    </tr>
    {% endfor%}
</table>

Prepared Games make it possible to create an immersive seamless experience for the players in a game with several rounds of play.