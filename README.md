#chat_menu {
    width: 300px
}

.channel_container {
    display: none;
    height: 350px;
    overflow-x: hidden;
    overflow-y: scroll
}

#chat_input {
    width: calc(100% - 10px)
}

.chat_channel {
    background-color: hsla(0,0%,100%,.067);
    border: none;
    margin-right: 2px;
    padding: 3px;
    text-transform: capitalize
}

.message_content {
    color: #fff
}

.message_content,.message_sender {
    cursor: text;
    -webkit-user-select: text;
    user-select: text
}

#message_title {
    color: #fff;
    font-size: 28px;
    margin: 0;
    text-align: center
}

#chat_notifications {
    background-color: #f73d3d;
    border-radius: 50%;
    bottom: 3px;
    color: #fff;
    display: inline-block;
    height: 20px;
    position: absolute;
    right: 3px;
    width: 20px
}

#clan_menu {
    width: 275px
}

#clan_list {
    height: 300px
}

#input_clan_name {
    background-color: hsla(0,0%,100%,.2);
    border: none;
    border-radius: 3px;
    color: #fff;
    font-size: 18px;
    margin-bottom: 3px;
    outline: none;
    padding: 0;
    width: 100%
}

.join_notification {
    background-color: rgba(0,0,0,.3);
    color: #fff;
    font-family: sans-serif;
    font-size: 20px;
    white-space: nowrap
}

.join_notification_accept {
    font-size: 20px;
    margin-left: 4px
}

.clan_container {
    background-color: rgba(0,0,0,.5);
    border-radius: 5px;
    margin: 5px;
    padding: 5px
}

.clan_action_button {
    display: inline-block;
    margin-left: 5px;
    margin-right: 5px;
    width: 100px
}

.clan_action_button_large {
    width: 100%
}

:root {
    --crafting-info-icon-size: 36px;
    --crafting-popup-width: 120px;
    --crafting-popup-half: calc(var(--crafting-popup-width)/2);
    --crafting-popup-top: calc(50vh + 200px - var(--crafting-popup-half));
    --crafting-popup-left: calc(50vw - var(--crafting-popup-half));
    --crafting-medium-zoom: 0.85;
    --crafting-small-zoom: 0.7;
    --crafting-small-width: 50px
}

#crafting_container {
    background-color: rgba(0,0,0,.533);
    left: 5px;
    overflow: auto;
    position: fixed;
    top: 5px;
    width: 200px
}

#crafting_container hr {
    border-color: #fff;
    margin: 0 0 4px
}

#crafting_categories {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around
}

#crafting_categories .category_image_container {
    cursor: pointer;
    height: 40px;
    padding-bottom: 2px;
    padding-top: 2px;
    transition: opacity .1s linear,transform .1s ease-out;
    width: 40px
}

#crafting_categories .category_image_container.selected_category {
    cursor: default;
    opacity: .5!important;
    transform: scale(.85)
}

#crafting_categories .category_image_container:hover {
    opacity: .7
}

#crafting_categories .category_image_container .category_image {
    width: 40px
}

#crafting_recipes {
    display: flex;
    flex-wrap: wrap
}

#crafting_recipes .recipe_image_container {
    align-items: center;
    cursor: pointer;
    display: flex;
    height: 50px;
    justify-content: center;
    position: relative;
    width: 50px
}

#crafting_recipes .recipe_image_container .favourite_icon {
    background-image: url(a5631238fa6f96471dc8.svg);
    background-size: 100%;
    bottom: 0;
    display: none;
    height: 20px;
    pointer-events: none;
    position: absolute;
    right: 0;
    width: 20px
}

#crafting_recipes .recipe_image_container.uncraftable {
    filter: brightness(.8) grayscale(.7);
    opacity: .8!important;
    order: 1
}

#crafting_recipes .recipe_image_container.favourite {
    order: 2
}

#crafting_recipes .recipe_image_container.favourite .favourite_icon {
    display: block
}

#crafting_recipes .recipe_image_container:hover {
    opacity: .7
}

#crafting_recipes .recipe_image_container .recipe_image {
    cursor: pointer;
    max-height: 50px;
    max-width: 50px
}

@keyframes popOut {
    0% {
        transform: scale(1)
    }

    50% {
        filter: drop-shadow(0 0 4px white);
        transform: scale(1.2)
    }

    to {
        transform: scale(1)
    }
}

.attach_crafting_container {
    display: none;
    font-size: 20px;
    left: 230px;
    position: fixed;
    top: 5px
}

#crafting_info_desc {
    background-color: rgba(34,34,34,.333);
    border: 1px solid hsla(0,0%,53%,.333);
    border-radius: 5px;
    color: #ccc;
    font-size: 14px;
    padding: 3px
}

#crafting_info_desc .item_desc_icon_container {
    align-items: center;
    display: inline-flex;
    height: 36px;
    height: var(--crafting-info-icon-size);
    justify-content: center;
    width: 36px;
    width: var(--crafting-info-icon-size)
}

#crafting_info_desc .item_desc_icon_container .item_desc_icon {
    max-height: 36px;
    max-height: var(--crafting-info-icon-size);
    max-width: 36px;
    max-width: var(--crafting-info-icon-size)
}

#crafting_info_desc .item_desc_attribute_container {
    align-items: center;
    display: inline-flex;
    height: 36px;
    height: var(--crafting-info-icon-size);
    justify-content: center;
    position: relative;
    width: 36px;
    width: var(--crafting-info-icon-size)
}

#crafting_info_desc .item_desc_attribute_container .item_desc_attribute_icon {
    left: 0;
    max-height: 25.2px;
    max-height: calc(var(--crafting-info-icon-size)*.7);
    max-width: 25.2px;
    max-width: calc(var(--crafting-info-icon-size)*.7);
    position: absolute;
    top: 0
}

#crafting_info_desc .item_desc_attribute_container .item_desc_attribute_number {
    bottom: 0;
    font-size: 18px;
    font-size: calc(var(--crafting-info-icon-size)/2);
    line-height: 24px;
    line-height: calc(var(--crafting-info-icon-size)/1.5);
    position: absolute;
    right: 4px;
    text-shadow: var(--text-outline)
}

.ingredient_count {
    font-size: 18px
}

.ingredient_count .ingredient_count_slash {
    color: #777;
    font-size: 14px
}

.ingredient_count .ingredient_count_current {
    color: #ddd;
    font-size: 14px
}

.ingredient_image {
    max-height: 14px
}

.big_popup {
    align-items: center;
    animation: bigPopup .4s ease-in-out infinite alternate;
    background-color: rgba(0,0,0,.267);
    border-radius: 24px;
    cursor: pointer;
    display: flex;
    height: 120px;
    justify-content: center;
    left: calc(50vw - 60px);
    left: var(--crafting-popup-left);
    outline: 4px solid hsla(0,0%,100%,.133);
    position: fixed;
    top: calc(50vh + 140px);
    top: var(--crafting-popup-top);
    width: 120px
}

.big_popup .icon {
    max-width: 80%
}

.big_popup.slide_away {
    animation: slideAway .5s ease-in
}

@keyframes bigPopup {
    0% {
        background-color: rgba(0,0,0,.133);
        outline-color: hsla(0,0%,100%,.133);
        transform: scale(1)
    }

    to {
        background-color: rgba(68,68,68,.133);
        outline-color: hsla(0,0%,100%,.4);
        transform: scale(1.1)
    }
}

@keyframes slideAway {
    0% {
        left: calc(50vw - 60px);
        left: var(--crafting-popup-left);
        opacity: 1;
        top: calc(50vh + 140px);
        top: var(--crafting-popup-top);
        transform: scale(1)
    }

    to {
        left: 0;
        opacity: 0;
        top: 0;
        transform: scale(0)
    }
}

@media screen and (max-height: 600px),screen and (max-width:850px) {
    #crafting_container {
        width:150px
    }

    #crafting_container,.attach_crafting_container {
        transform: scale(.85);
        transform: scale(var(--crafting-medium-zoom));
        transform-origin: top left
    }

    .attach_crafting_container {
        left: 153px;
        left: calc(180px*var(--crafting-medium-zoom))
    }
}

@media screen and (max-height: 400px),screen and (max-width:700px) {
    #crafting_container {
        width:100px
    }

    #crafting_container,.attach_crafting_container {
        transform: scale(.7);
        transform: scale(var(--crafting-small-zoom));
        transform-origin: top left
    }

    .attach_crafting_container {
        left: 91px;
        left: calc(130px*var(--crafting-small-zoom))
    }
}

@media screen and (max-width: 500px) {
    #crafting_container {
        border-radius:0;
        height: 142.85714vh;
        height: calc(100vh/var(--crafting-small-zoom));
        left: 0;
        padding: 6px;
        top: 0;
        width: 50px;
        width: var(--crafting-small-width)
    }

    #crafting_container #crafting_categories .category_image_container {
        display: none
    }

    #crafting_container #crafting_categories .category_image_container.selected_category {
        cursor: pointer!important;
        display: block;
        opacity: 1!important;
        transform: none!important
    }

    #crafting_container.mobile_view_categories .category_image_container {
        display: block!important
    }

    #crafting_container.mobile_view_categories .recipe_image_container {
        display: none!important
    }

    #crafting_container.mobile_view_categories hr {
        display: none
    }

    .attach_crafting_container {
        left: 80px;
        top: 5px
    }
}

#death_animation {
    animation: deathanimation 3s cubic-bezier(.6,0,.4,1);
    background-color: #000;
    display: none;
    height: 100vh;
    -webkit-mask: url(e42b561fa91b3db46c79.svg);
    mask: url(e42b561fa91b3db46c79.svg);
    -webkit-mask-position: 50% 50%;
    mask-position: 50% 50%;
    -webkit-mask-repeat: no-repeat;
    mask-repeat: no-repeat;
    position: fixed;
    width: 100vw;
    z-index: 999
}

@keyframes deathanimation {
    0% {
        -webkit-mask-size: 500000px;
        mask-size: 500000px
    }

    40% {
        -webkit-mask-size: 7000px;
        mask-size: 7000px
    }

    60% {
        -webkit-mask-size: 7000px;
        mask-size: 7000px
    }

    to {
        -webkit-mask-size: 500000px;
        mask-size: 500000px
    }
}

#death_screen {
    font-size: 20px;
    padding: 10px
}

#death_screen::backdrop {
    background-color: rgba(0,0,0,.267)
}

#death_screen p {
    margin: 2px
}

#death_screen_red {
    color: red
}

#death_screen_title {
    font-size: 38px;
    text-align: center
}

#death_screen_close {
    border-radius: 5px;
    cursor: pointer;
    padding: 10px;
    position: absolute;
    right: 0;
    top: 0
}

#death_screen_close:hover {
    background-color: hsla(0,0%,100%,.133)
}

#top_right {
    position: fixed;
    right: 5px;
    top: 5px
}

#top_right #top_right_icons {
    display: flex;
    flex-direction: row-reverse;
    gap: 3px
}

#top_right #top_right_icons .ingame_button {
    background-color: rgba(0,0,0,.533);
    border: none;
    border-radius: 5px;
    color: #fff;
    font-size: 1em;
    height: 50px;
    position: relative;
    width: 50px
}

#top_right #top_right_icons .ingame_button:hover {
    background-color: rgba(68,68,68,.533)
}

#top_right #top_right_icons .ingame_button img {
    margin: 3px;
    pointer-events: none
}

#top_right #leaderboard_container {
    background-color: rgba(0,0,0,.533);
    border-radius: 5px;
    margin-bottom: 3px;
    margin-top: 3px;
    padding: 3px;
    width: 200px
}

#top_right #leaderboard_container .leaderboard_row {
    color: #fff;
    display: flex;
    font-size: 1.2em;
    height: 24px;
    justify-content: space-between;
    line-height: 24px;
    margin: 2px
}

#top_right #leaderboard_container .leaderboard_row.self {
    color: #ff0
}

#top_right #leaderboard_container .leaderboard_row .left_text {
    max-width: 150px;
    overflow: hidden;
    text-overflow: "..";
    white-space: nowrap
}

#top_right #leaderboard_container .leaderboard_row .right_text {
    max-width: 50px
}

#top_right #leaderboard_container .leaderboard_row .right_text .kills_text {
    display: none
}

#top_right #leaderboard_container:hover .kills_text {
    display: block!important
}

#top_right #leaderboard_container:hover .score_text {
    display: none
}

@media (max-width: 700px) {
    #top_right #leaderboard_container {
        display:none
    }
}

.user_info_button {
    border: 1px solid #fff;
    border-radius: 5px;
    display: inline;
    margin: 2px;
    padding: 3px 5px
}

.option_label {
    color: #fff
}

#options_menu label,.option_label {
    vertical-align: top
}

.item_description_container {
    background-color: hsla(0,0%,100%,.1);
    border-radius: 5px;
    color: #ddd;
    margin-bottom: 10px;
    padding: 5px
}

.item_cost_text {
    color: #ddd;
    display: inline
}

.item_cost_img {
    display: inline;
    height: 16px;
    width: 16px
}

@media screen and (max-height: 600px),screen and (max-width:800px) {
    #top_right {
        transform:scale(.85);
        transform-origin: top right
    }
}

@media screen and (max-height: 500px),screen and (max-width:700px) {
    #top_right {
        transform:scale(.7);
        transform-origin: top right
    }
}

@font-face {
    font-family: HammersmithOne;
    src: url(f6b0809dd1f395240bc4.ttf) format("truetype")
}

body {
    margin: 0;
    overflow: hidden
}

body * {
    font-family: HammersmithOne
}

p {
    margin-bottom: 0;
    margin-top: 0
}

img {
    pointer-events: none
}

.unselectable {
    -webkit-user-select: none;
    user-select: none
}

button {
    cursor: pointer
}

button:disabled {
    cursor: not-allowed
}

dialog {
    -webkit-backdrop-filter: blur(4px);
    backdrop-filter: blur(4px);
    border: none;
    box-shadow: none;
    outline: none
}

:root {
    --inventory-rows: 2;
    --inventory-columns: 8;
    --inventory-slot-size: min(60px,calc(100vw/var(--inventory-columns) - 10px),calc(30vh/var(--inventory-rows) - 10px));
    --inventory-hotbar-background: rgba(0,0,0,.4);
    --inventory-slot-background: rgba(0,0,0,.2);
    --inventory-slot-background-omitted: rgba(0,0,0,.067);
    --inventory-container-width: calc((var(--inventory-slot-size) + 2px)*var(--inventory-columns));
    --text-outline: -1px -1px 0 #000,1px -1px 0 #000,-1px 1px 0 #000,1px 1px 0 #000,-1.414px 0 0 #000,1.414px 0 0 #000,0 -1.414px 0 #000,0 1.414px 0 #000;
    --text-size: max(calc(var(--inventory-slot-size)/3),11px);
    --inventory-info-icon-size: 40px;
    --drop-scale: min(1.5vw,10px);
    --drop-container-width: calc(var(--drop-scale)*20);
    --drop-img-width: calc(var(--drop-scale)*4);
    --drop-option-width: calc(var(--drop-scale)*7);
    --drop-text-size: calc(var(--drop-scale)*2.4)
}

#inventory_container {
    align-content: flex-start;
    bottom: 2px;
    display: flex;
    flex-wrap: wrap-reverse;
    gap: 2px;
    justify-content: center;
    left: calc(50% - (min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px)) + 2px)*8/2);
    left: calc(50% - min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))*8/2 - 8px);
    left: calc(50% - var(--inventory-container-width)/2);
    position: fixed;
    text-align: center;
    width: calc((min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px)) + 2px)*8);
    width: calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))*8 + 16px);
    width: var(--inventory-container-width)
}

#inventory_container .inventory_slot {
    align-items: center;
    background-color: rgba(0,0,0,.4);
    background-color: var(--inventory-hotbar-background);
    border-radius: calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))/5);
    border-radius: calc(var(--inventory-slot-size)/5);
    cursor: pointer;
    display: inline-flex;
    flex: 0 0 min(60px,calc(12.5vw - 10px),calc(15vh - 10px));
    flex: 0 0 var(--inventory-slot-size);
    height: min(60px,calc(12.5vw - 10px),calc(15vh - 10px));
    height: var(--inventory-slot-size);
    justify-content: center;
    position: relative;
    transition: background-color .1s ease-out,outline .1s linear,opacity .1s linear;
    width: min(60px,calc(12.5vw - 10px),calc(15vh - 10px));
    width: var(--inventory-slot-size)
}

#inventory_container .inventory_slot .icon {
    max-height: 90%;
    max-width: 90%
}

#inventory_container .inventory_slot .item_count {
    bottom: 0;
    color: #fff;
    font-size: max(calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))/3),11px);
    font-size: var(--text-size);
    line-height: max(calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))/3),11px);
    line-height: var(--text-size);
    pointer-events: none;
    position: absolute;
    right: 0;
    text-shadow: -1px -1px 0 #000,1px -1px 0 #000,-1px 1px 0 #000,1px 1px 0 #000,-1.414px 0 0 #000,1.414px 0 0 #000,0 -1.414px 0 #000,0 1.414px 0 #000;
    text-shadow: var(--text-outline)
}

#inventory_container .inventory_slot.selected {
    background-color: hsla(0,0%,87%,.267);
    outline: 2px solid hsla(0,0%,100%,.533)
}

#inventory_container .inventory_slot.omitted {
    background-color: rgba(0,0,0,.067);
    background-color: var(--inventory-slot-background-omitted);
    opacity: .85
}

#inventory_container .inventory_info {
    background-color: rgba(0,0,0,.4);
    border: 2px solid hsla(0,0%,100%,.267);
    border-radius: calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))/5);
    border-radius: calc(var(--inventory-slot-size)/5);
    bottom: 100%;
    color: #fff;
    display: none;
    font-size: 20px;
    left: 0;
    margin-bottom: 4px;
    max-width: 270px;
    outline: 2px solid hsla(0,0%,100%,.067);
    padding: 8px;
    pointer-events: none;
    position: absolute;
    text-align: left
}

#inventory_container .inventory_info .item_desc_icon_container {
    align-items: center;
    display: inline-flex;
    height: 40px;
    height: var(--inventory-info-icon-size);
    justify-content: center;
    width: 40px;
    width: var(--inventory-info-icon-size)
}

#inventory_container .inventory_info .item_desc_icon_container .item_desc_icon {
    max-height: 40px;
    max-height: var(--inventory-info-icon-size);
    max-width: 40px;
    max-width: var(--inventory-info-icon-size)
}

#inventory_container .inventory_info .item_desc_attribute_container {
    align-items: center;
    display: inline-flex;
    height: 40px;
    height: var(--inventory-info-icon-size);
    justify-content: center;
    position: relative;
    width: 40px;
    width: var(--inventory-info-icon-size)
}

#inventory_container .inventory_info .item_desc_attribute_container .item_desc_attribute_icon {
    left: 0;
    max-height: 28px;
    max-height: calc(var(--inventory-info-icon-size)*.7);
    max-width: 28px;
    max-width: calc(var(--inventory-info-icon-size)*.7);
    position: absolute;
    top: 0
}

#inventory_container .inventory_info .item_desc_attribute_container .item_desc_attribute_number {
    bottom: 0;
    font-size: calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))/3.5);
    font-size: calc(var(--inventory-slot-size)/3.5);
    position: absolute;
    right: 4px;
    text-shadow: -1px -1px 0 #000,1px -1px 0 #000,-1px 1px 0 #000,1px 1px 0 #000,-1.414px 0 0 #000,1.414px 0 0 #000,0 -1.414px 0 #000,0 1.414px 0 #000;
    text-shadow: var(--text-outline)
}

#inventory_container:hover .omitted {
    background-color: rgba(0,0,0,.2);
    background-color: var(--inventory-slot-background);
    opacity: 1
}

.drag_preview {
    max-height: min(60px,calc(12.5vw - 10px),calc(15vh - 10px));
    max-height: var(--inventory-slot-size);
    max-width: min(60px,calc(12.5vw - 10px),calc(15vh - 10px));
    max-width: var(--inventory-slot-size);
    pointer-events: none;
    position: fixed;
    transform: translate(-50%,-50%)
}

#status_effect_container {
    background-color: rgba(0,0,0,.2);
    background-color: var(--inventory-slot-background);
    border-radius: 5px;
    bottom: calc(min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))*2 + 6px);
    bottom: calc(var(--inventory-slot-size)*var(--inventory-rows) + 6px);
    display: flex;
    position: fixed;
    right: calc(50% - (min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px)) + 2px)*8/2);
    right: calc(50% - min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))*8/2 - 8px);
    right: calc(50% - var(--inventory-container-width)/2)
}

#status_effect_container .status_effect {
    cursor: pointer;
    display: none;
    max-height: 32px;
    max-width: 32px
}

#status_effect_container .status_effect .status_effect_ico {
    height: 90%;
    margin: 5%;
    width: 90%
}

#status_effect_container .status_effect.urgent .status_effect_ico {
    animation: urgent .5s ease-in-out infinite alternate
}

#status_effect_container .status_effect .status_effect_info {
    background-color: rgba(0,0,0,.2);
    background-color: var(--inventory-slot-background);
    border-radius: 5px;
    bottom: 36px;
    color: #fff;
    display: none;
    padding: 3px;
    position: absolute;
    right: 0;
    white-space: nowrap
}

#status_effect_container .status_effect:hover .status_effect_info {
    display: block
}

@keyframes urgent {
    0% {
        filter: "";
        opacity: .3;
        transform: scale(.8)
    }

    to {
        filter: sepia(1) hue-rotate(-25deg) saturate(2);
        opacity: 1;
        transform: scale(1)
    }
}

.admin_con {
    left: 0;
    margin: 100px;
    padding: 100px;
    pointer-events: none;
    position: fixed;
    top: 0
}

.admin_con .admin_item_con {
    align-items: center;
    display: inline-flex;
    height: 60px;
    justify-content: center;
    width: 60px
}

.admin_con .admin_item_con .admin_item {
    cursor: pointer;
    max-height: 100%;
    max-width: 100%;
    pointer-events: all
}

.admin_con .admin_item_con .admin_item:hover {
    background-color: hsla(0,0%,100%,.133)
}

.drop_container {
    background-color: rgba(0,0,0,.133);
    border-radius: 50%;
    height: calc(min(1.5vw, 10px)*20);
    height: var(--drop-container-width);
    position: fixed;
    transform: translate(-50%,-50%);
    width: calc(min(1.5vw, 10px)*20);
    width: var(--drop-container-width)
}

.drop_container .item_preview {
    left: 50%;
    max-width: calc(min(1.5vw, 10px)*4);
    max-width: var(--drop-img-width);
    pointer-events: all;
    top: 50%
}

.drop_container .drop_option,.drop_container .item_preview {
    cursor: pointer;
    position: absolute;
    transform: translate(-50%,-50%)
}

.drop_container .drop_option {
    align-items: center;
    background-color: rgba(0,0,0,.267);
    border-radius: 50%;
    display: flex;
    height: calc(min(1.5vw, 10px)*7);
    height: var(--drop-option-width);
    justify-content: center;
    overflow: hidden;
    width: calc(min(1.5vw, 10px)*7);
    width: var(--drop-option-width)
}

.drop_container .drop_option .drop_text {
    color: #fff;
    font-size: calc(min(1.5vw, 10px)*2.4);
    font-size: var(--drop-text-size);
    text-shadow: -1px -1px 0 #000,1px -1px 0 #000,-1px 1px 0 #000,1px 1px 0 #000,-1.414px 0 0 #000,1.414px 0 0 #000,0 -1.414px 0 #000,0 1.414px 0 #000;
    text-shadow: var(--text-outline);
    z-index: 1
}

.drop_container .drop_option:hover {
    background-color: hsla(0,0%,87%,.267)
}

.drop_container .drop_option .drop_portion {
    background-color: hsla(0,0%,100%,.533);
    bottom: 0;
    left: 0;
    position: absolute;
    width: 100%
}

@media screen and (max-width: 500px) {
    #inventory_container {
        left:calc(50% + var(--crafting-small-width)/2*var(--crafting-small-zoom) - (min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px)) + 2px)*8/2);
        left: calc(50% + var(--crafting-small-width)/2*var(--crafting-small-zoom) - min(60px, calc(100vw / 8 - 10px), calc(30vh / 2 - 10px))*8/2 - 8px);
        left: calc(50% + var(--crafting-small-width)/2*var(--crafting-small-zoom) - var(--inventory-container-width)/2)
    }
}

.menu_container {
    align-items: center;
    display: flex;
    height: 100vh;
    justify-content: center;
    left: 0;
    pointer-events: none;
    position: fixed;
    top: 0;
    width: 100vw
}

.menu_container .ingame_draggable_menu {
    background-color: rgba(0,0,0,.4);
    border-radius: 5px;
    box-shadow: 2px 2px 2px rgba(0,0,0,.067);
    cursor: grab;
    padding-top: 22px;
    pointer-events: all;
    position: relative;
    transition: box-shadow .2s ease-out
}

.menu_container .ingame_draggable_menu.dragged_window {
    box-shadow: 10px 10px 10px rgba(0,0,0,.267)
}

.menu_container .ingame_draggable_menu .close {
    background-image: url(e349d94d646535e8670d.svg);
    cursor: pointer;
    height: 18px;
    position: absolute;
    right: 2px;
    top: -22px;
    width: 18px
}

.menu_container .ingame_draggable_menu .close:hover {
    background-color: hsla(0,0%,100%,.133)
}

.menu_container .ingame_draggable_menu .ingame_menu {
    background-color: rgba(0,0,0,.133);
    border-radius: 0 0 5px 5px;
    border-top: 3px solid hsla(0,0%,100%,.067);
    color: hsla(0,0%,100%,.6);
    cursor: default;
    font-family: sans-serif;
    font-size: 18px;
    padding: 10px;
    pointer-events: all;
    position: relative;
    width: auto
}

@media screen and (max-height: 700px),screen and (max-width:600px) {
    .ingame_draggable_menu {
        transform:scale(.85)
    }
}

@media screen and (max-height: 500px),screen and (max-width:450px) {
    .ingame_draggable_menu {
        transform:scale(.7)
    }
}

:root {
    --minimap-size: 12.5vw;
    --minimap-marker: 1vw
}

#bottom_right {
    bottom: 0;
    position: fixed;
    right: 0
}

#bottom_right #minimap {
    cursor: crosshair;
    height: 12.5vw;
    height: var(--minimap-size);
    position: relative;
    width: 12.5vw;
    width: var(--minimap-size)
}

#bottom_right #minimap .custom_marker {
    cursor: pointer;
    pointer-events: all;
    position: absolute;
    transform: translate(-50%,-50%);
    width: 1vw;
    width: var(--minimap-marker)
}

#bottom_right #show_on_map {
    background-color: rgba(0,0,0,.733);
    border-top-left-radius: 4px;
    color: #fff;
    font-size: 1.4vw;
    margin: 0;
    white-space: nowrap;
    width: 12.5vw
}

#bottom_right #show_on_map #show_on_map_check {
    cursor: pointer;
    height: 20px;
    vertical-align: middle;
    width: 20px
}

@media (max-width: 750px) {
    #bottom_right {
        display:none
    }
}

.centered_text {
    left: 50%;
    position: absolute;
    top: 50%;
    transform: translateX(-50%) translateY(-50%)
}

.vertical_flip {
    transform: scaleY(-1)
}

.horizontal_flip {
    transform: scaleX(-1)
}

.center_text {
    align-items: center;
    display: flex;
    justify-content: center
}

.smooth_button {
    background-color: hsla(0,0%,100%,.2);
    border: none;
    border-radius: 3px;
    color: #fff;
    height: 30px
}

.rounded {
    border-radius: 5px;
    padding: 5px
}

.darkbox {
    background-color: rgba(0,0,0,.7);
    border-radius: 5px;
    color: #fff;
    padding: 10px
}

::-webkit-scrollbar {
    width: 5px
}

::-webkit-scrollbar,::-webkit-scrollbar-track {
    background-color: transparent
}

::-webkit-scrollbar-thumb {
    background-color: hsla(0,0%,53%,.733);
    border-radius: 4px
}

::-webkit-scrollbar-thumb:hover {
    background-color: #aaa
}

@keyframes fadeIn {
    0% {
        opacity: 0
    }

    to {
        opacity: 1
    }
}

#titleBackground {
    background-image: url(136a5eb00c5fee62eca2.svg);
    background-repeat: repeat;
    background-size: cover;
    height: 100%;
    overflow: hidden;
    padding-top: 8px;
    pointer-events: none;
    position: absolute;
    width: 101%;
    z-index: -1
}

#titleBackground #moon {
    --distance: min(50vw,350px);
    animation: moonGlide 100s linear infinite;
    background-color: #e3debe;
    border-radius: 50%;
    height: 200px;
    left: 50%;
    position: absolute;
    width: 200px
}

#titleBackground .fog {
    --svg-width: 1734px;
    animation: var(--duration) fogGlide infinite reverse linear var(--delay);
    background-image: url(8d426673267d288e0c12.svg);
    background-repeat: repeat-x;
    background-size: auto 100%;
    bottom: var(--offset);
    height: 150px;
    position: absolute;
    width: calc(100vw + 1734px);
    width: calc(100vw + var(--svg-width))
}

#titleBackground .fogTop {
    top: var(--offset)!important
}

#titleBackground .stones {
    background-position-y: bottom;
    background-repeat: repeat-x;
    bottom: var(--offset);
    height: 340px;
    position: absolute;
    width: 100%
}

#titleBackground .stone1 {
    background-image: url(a1ffc0ca8dc2d4223fad.svg)
}

#titleBackground .stone2 {
    background-image: url(8b9284eed41aa6135347.svg)
}

#titleBackground .stone3 {
    background-image: url(c28b02a282e0105acc65.svg)
}

#titleBackground #tower {
    bottom: 300px;
    left: 10%;
    position: absolute
}

#titleBackground #lava {
    --svg-width: 2228px;
    animation: lavaGlide 50s linear infinite;
    background-image: url(49fa7fe93bd67b027420.svg);
    background-size: auto;
    bottom: 43px;
    height: 200px;
    position: absolute;
    width: calc(100vw + 2228px);
    width: calc(100vw + var(--svg-width))
}

@keyframes moonGlide {
    0% {
        transform: translateX(calc(var(--distance)*-1 - 50%))
    }

    to {
        transform: translateX(calc(var(--distance) - 50%))
    }
}

@keyframes fogGlide {
    0% {
        transform: translateX(calc(0px - var(--svg-width)))
    }

    to {
        transform: translateX(0)
    }
}

@keyframes lavaGlide {
    0% {
        transform: translateX(calc(0px - var(--svg-width)))
    }

    to {
        transform: translateX(0)
    }
}

#input_username {
    background-color: rgba(0,0,0,.3);
    border: none;
    border-radius: 5px;
    color: #fff;
    font-size: 20px;
    outline: none;
    padding: 10px;
    width: 200px
}

#content {
    align-items: center;
    display: flex;
    flex-direction: column
}

#content #title {
    animation: fadeIn 1s linear;
    margin: 1em 0;
    max-width: 85%
}

#content #title_small {
    border-radius: 10px;
    box-shadow: 1px 1px 3px #000;
    display: none;
    left: 10px;
    position: fixed;
    top: 10px;
    z-index: -1
}

#content .darkbox {
    box-shadow: 0 5px 0 0 rgba(0,0,0,.2)
}

#content #connect_button {
    background-color: orange;
    border: none;
    border-radius: 5px;
    color: #fff;
    font-size: 20px;
    outline: none;
    overflow: hidden;
    padding: 10px;
    position: relative;
    width: 75px
}

#content #connect_button:hover {
    background-color: #ff9000
}

#content #connect_button:disabled {
    background-color: grey
}

#content #connect_button #loading_progress {
    background-color: hsla(0,0%,100%,.267);
    height: 100%;
    left: 0;
    position: absolute;
    top: 0;
    width: 0
}

#content #footer {
    background-color: rgba(0,0,0,.5);
    border-radius: 10px 10px 0 0;
    bottom: 0;
    column-gap: 1.5em;
    display: flex;
    font-size: 1.2em;
    list-style-type: none;
    margin: 0;
    padding: .2em 1em 0;
    position: absolute
}

#content #footer a,#content #footer button {
    color: #fff;
    cursor: pointer;
    display: inline-block;
    -webkit-text-decoration: none;
    text-decoration: none
}

#content #footer a:hover,#content #footer button:hover {
    opacity: .8
}

#content #footer a * {
    vertical-align: top
}

#content #footer button {
    background-color: transparent;
    border: none;
    font-size: 100%;
    padding: 0
}

@media screen and (max-width: 600px) {
    #footer {
        border-radius:0!important;
        display: block!important;
        left: 0;
        width: 100%!important
    }

    #footer a,#footer button {
        display: block!important;
        margin: 4px 15px!important
    }
}

#doomed-io_300x250 {
    background-color: hsla(0,0%,100%,.5);
    display: block;
    height: 250px;
    margin: 0 auto;
    width: 300px
}

.ad:before {
    content: "Advertisement";
    display: block;
    font-size: .8em;
    font-weight: thin;
    text-align: center
}

@media screen and (max-height: 700px) {
    #title {
        max-height:calc(100vh - 500px)
    }
}

@media screen and (max-height: 550px) {
    #title {
        display:none
    }

    #title_small {
        display: block!important
    }

    #main-page {
        align-items: center;
        display: flex;
        height: 100vh
    }

    #footer {
        flex-direction: column;
        margin: 4px;
        padding: .2em!important;
        right: 0
    }
}

:root {
    --toast-width: max(300px,min(40vw,600px));
    --toast-height: 150px
}

.toast {
    animation: toastAnim 3.5s ease-in-out;
    bottom: 100vh;
    font-size: 1.5em;
    max-height: 150px;
    max-height: var(--toast-height);
    position: fixed
}

.toast.darkbox {
    left: calc(50vw - max(300px, min(40vw, 600px))/2);
    left: calc(50vw - var(--toast-width)/2);
    width: max(300px,min(40vw,600px));
    width: var(--toast-width)
}

.toast.toastimg {
    left: 50vw;
    translate: -50%
}

@keyframes toastAnim {
    0% {
        bottom: 100vh
    }

    20% {
        bottom: calc(100vh - 150px);
        bottom: calc(100vh - var(--toast-height))
    }

    80% {
        bottom: calc(100vh - 150px);
        bottom: calc(100vh - var(--toast-height))
    }

    to {
        bottom: 100vh
    }
}

.tooltip {
    border-bottom: 1px dotted #000;
    display: inline-block;
    position: relative
}

.tooltip .tooltiptext {
    background-color: #555;
    border-radius: 6px;
    bottom: 125%;
    color: #fff;
    left: 50%;
    margin-left: -60px;
    opacity: 0;
    padding: 5px 0;
    position: absolute;
    text-align: center;
    transition: opacity 1s;
    visibility: hidden;
    width: 120px;
    z-index: 1
}

.tooltip .tooltiptext:after {
    border: 5px solid transparent;
    border-top-color: #555;
    content: "";
    left: 50%;
    margin-left: -5px;
    position: absolute;
    top: 100%
}

.tooltip:hover .tooltiptext {
    opacity: 1;
    visibility: visible
}
