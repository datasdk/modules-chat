<<<<<<< HEAD
﻿<!-- DATAS_API_README:START -->
# Chat Module

Automatisk genereret API-README for `Chat` modulet.

- **Alias:** `chat`
- **Antal API-routes:** `30`
- **Genereret:** `2026-05-12 22:32:06`
- **Modulbeskrivelse:** API- og funktionsmodul for Chat.
- **Providers:** `Modules\Chat\Providers\ChatServiceProvider`

## API-kald

### `GET|HEAD` `/api/chats/conversations`

- **Sti:** `/api/chats/conversations`
- **Method:** `GET|HEAD`
- **Beskrivelse:** Henter en pagineret liste.
- **Output i data:** `data`: pagineret liste af Conversation med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@index`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.index`

### `POST` `/api/chats/conversations`

- **Sti:** `/api/chats/conversations`
- **Method:** `POST`
- **Beskrivelse:** Opretter en ny ressource.
- **Output i data:** `data`: oprettet Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@store`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.store`

### `DELETE` `/api/chats/conversations/batch`

- **Sti:** `/api/chats/conversations/batch`
- **Method:** `DELETE`
- **Beskrivelse:** Sletter flere ressourcer i en batch.
- **Output i data:** `data`: batch-resultat for slettede ressourcer.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@batchDestroy`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.batchDestroy`

### `PATCH` `/api/chats/conversations/batch`

- **Sti:** `/api/chats/conversations/batch`
- **Method:** `PATCH`
- **Beskrivelse:** Opdaterer flere ressourcer i en batch.
- **Output i data:** `data`: opdateret Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@batchUpdate`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.batchUpdate`

### `POST` `/api/chats/conversations/batch`

- **Sti:** `/api/chats/conversations/batch`
- **Method:** `POST`
- **Beskrivelse:** Opretter flere ressourcer i en batch.
- **Output i data:** `data`: oprettet Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@batchStore`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.batchStore`

### `POST` `/api/chats/conversations/search`

- **Sti:** `/api/chats/conversations/search`
- **Method:** `POST`
- **Beskrivelse:** Søger og filtrerer ressourcer.
- **Output i data:** `data`: pagineret liste af Conversation med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@search`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.search`

### `DELETE` `/api/chats/conversations/{conversation}`

- **Sti:** `/api/chats/conversations/{conversation}`
- **Method:** `DELETE`
- **Beskrivelse:** Sletter en ressource.
- **Output i data:** HTTP 204 uden body eller `data: { message: string }`, afhængigt af controller.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@destroy`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.destroy`

### `GET|HEAD` `/api/chats/conversations/{conversation}`

- **Sti:** `/api/chats/conversations/{conversation}`
- **Method:** `GET|HEAD`
- **Beskrivelse:** Henter en enkelt ressource.
- **Output i data:** `data`: Conversation-objekt med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@show`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.show`

### `PUT|PATCH` `/api/chats/conversations/{conversation}`

- **Sti:** `/api/chats/conversations/{conversation}`
- **Method:** `PUT|PATCH`
- **Beskrivelse:** Opdaterer en eksisterende ressource.
- **Output i data:** `data`: opdateret Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\ConversationController@update`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.update`

### `GET|HEAD` `/api/chats/conversations/{conversation}/messages`

- **Sti:** `/api/chats/conversations/{conversation}/messages`
- **Method:** `GET|HEAD`
- **Beskrivelse:** Henter en pagineret liste.
- **Output i data:** `data`: pagineret liste af Conversation med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@index`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.index`

### `POST` `/api/chats/conversations/{conversation}/messages`

- **Sti:** `/api/chats/conversations/{conversation}/messages`
- **Method:** `POST`
- **Beskrivelse:** Opretter en ny ressource.
- **Output i data:** `data`: oprettet Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@store`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.store`

### `POST` `/api/chats/conversations/{conversation}/messages/associate`

- **Sti:** `/api/chats/conversations/{conversation}/messages/associate`
- **Method:** `POST`
- **Beskrivelse:** Tilknytter en relateret ressource.
- **Output i data:** `data`: JSON-respons fra controlleren for Conversation.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@associate`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.associate`

### `DELETE` `/api/chats/conversations/{conversation}/messages/batch`

- **Sti:** `/api/chats/conversations/{conversation}/messages/batch`
- **Method:** `DELETE`
- **Beskrivelse:** Sletter flere ressourcer i en batch.
- **Output i data:** `data`: batch-resultat for slettede ressourcer.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@batchDestroy`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.batchDestroy`

### `PATCH` `/api/chats/conversations/{conversation}/messages/batch`

- **Sti:** `/api/chats/conversations/{conversation}/messages/batch`
- **Method:** `PATCH`
- **Beskrivelse:** Opdaterer flere ressourcer i en batch.
- **Output i data:** `data`: opdateret Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@batchUpdate`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.batchUpdate`

### `POST` `/api/chats/conversations/{conversation}/messages/batch`

- **Sti:** `/api/chats/conversations/{conversation}/messages/batch`
- **Method:** `POST`
- **Beskrivelse:** Opretter flere ressourcer i en batch.
- **Output i data:** `data`: oprettet Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@batchStore`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.batchStore`

### `POST` `/api/chats/conversations/{conversation}/messages/search`

- **Sti:** `/api/chats/conversations/{conversation}/messages/search`
- **Method:** `POST`
- **Beskrivelse:** Søger og filtrerer ressourcer.
- **Output i data:** `data`: pagineret liste af Conversation med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@search`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.search`

### `DELETE` `/api/chats/conversations/{conversation}/messages/{message?}`

- **Sti:** `/api/chats/conversations/{conversation}/messages/{message?}`
- **Method:** `DELETE`
- **Beskrivelse:** Sletter en ressource.
- **Output i data:** HTTP 204 uden body eller `data: { message: string }`, afhængigt af controller.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@destroy`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.destroy`

### `GET|HEAD` `/api/chats/conversations/{conversation}/messages/{message?}`

- **Sti:** `/api/chats/conversations/{conversation}/messages/{message?}`
- **Method:** `GET|HEAD`
- **Beskrivelse:** Henter en enkelt ressource.
- **Output i data:** `data`: Conversation-objekt med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@show`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.show`

### `PUT|PATCH` `/api/chats/conversations/{conversation}/messages/{message?}`

- **Sti:** `/api/chats/conversations/{conversation}/messages/{message?}`
- **Method:** `PUT|PATCH`
- **Beskrivelse:** Opdaterer en eksisterende ressource.
- **Output i data:** `data`: opdateret Conversation-objekt eller batch-resultat med modelens felter. Mulige `include` relationer: `messages`, `last_message`, `participants.messageable`, `participants`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@update`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.update`

### `DELETE` `/api/chats/conversations/{conversation}/messages/{message?}/dissociate`

- **Sti:** `/api/chats/conversations/{conversation}/messages/{message?}/dissociate`
- **Method:** `DELETE`
- **Beskrivelse:** Fjerner en relation til en ressource.
- **Output i data:** `data`: JSON-respons fra controlleren for Conversation.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@dissociate`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.conversations.messages.dissociate`

### `GET|HEAD` `/api/chats/members`

- **Sti:** `/api/chats/members`
- **Method:** `GET|HEAD`
- **Beskrivelse:** Henter en pagineret liste.
- **Output i data:** `data`: pagineret liste af Participation med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@index`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.index`

### `POST` `/api/chats/members`

- **Sti:** `/api/chats/members`
- **Method:** `POST`
- **Beskrivelse:** Opretter en ny ressource.
- **Output i data:** `data`: oprettet Participation-objekt eller batch-resultat med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@store`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.store`

### `DELETE` `/api/chats/members/batch`

- **Sti:** `/api/chats/members/batch`
- **Method:** `DELETE`
- **Beskrivelse:** Sletter flere ressourcer i en batch.
- **Output i data:** `data`: batch-resultat for slettede ressourcer.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@batchDestroy`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.batchDestroy`

### `PATCH` `/api/chats/members/batch`

- **Sti:** `/api/chats/members/batch`
- **Method:** `PATCH`
- **Beskrivelse:** Opdaterer flere ressourcer i en batch.
- **Output i data:** `data`: opdateret Participation-objekt eller batch-resultat med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@batchUpdate`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.batchUpdate`

### `POST` `/api/chats/members/batch`

- **Sti:** `/api/chats/members/batch`
- **Method:** `POST`
- **Beskrivelse:** Opretter flere ressourcer i en batch.
- **Output i data:** `data`: oprettet Participation-objekt eller batch-resultat med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@batchStore`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.batchStore`

### `POST` `/api/chats/members/search`

- **Sti:** `/api/chats/members/search`
- **Method:** `POST`
- **Beskrivelse:** Søger og filtrerer ressourcer.
- **Output i data:** `data`: pagineret liste af Participation med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@search`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.search`

### `DELETE` `/api/chats/members/{member}`

- **Sti:** `/api/chats/members/{member}`
- **Method:** `DELETE`
- **Beskrivelse:** Sletter en ressource.
- **Output i data:** HTTP 204 uden body eller `data: { message: string }`, afhængigt af controller.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@destroy`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.destroy`

### `GET|HEAD` `/api/chats/members/{member}`

- **Sti:** `/api/chats/members/{member}`
- **Method:** `GET|HEAD`
- **Beskrivelse:** Henter en enkelt ressource.
- **Output i data:** `data`: Participation-objekt med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@show`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.show`

### `PUT|PATCH` `/api/chats/members/{member}`

- **Sti:** `/api/chats/members/{member}`
- **Method:** `PUT|PATCH`
- **Beskrivelse:** Opdaterer en eksisterende ressource.
- **Output i data:** `data`: opdateret Participation-objekt eller batch-resultat med conversation_id, messageable_id, messageable_type. Mulige `include` relationer: `user`, `user.company`.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MembersController@update`
- **Request:** `Ikke angivet`
- **Resource:** `BaseResource/JSON`
- **Route name:** `api.chats.members.update`

### `POST` `/api/chats/{id}/message/send`

- **Sti:** `/api/chats/{id}/message/send`
- **Method:** `POST`
- **Beskrivelse:** Sender data eller notifikation via modulets service.
- **Output i data:** `data`: JSON-respons fra controlleren for Conversation.
- **Auth:** Kræver API-auth
- **Controller:** `Modules\Chat\Http\Controllers\Api\MessageController@send`
- **Request:** `ChatRequest`
- **Resource:** `ChatResource`
- **Route name:** `api.chats.`

<!-- DATAS_API_README:END -->
=======
<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
>>>>>>> f7956370a82e65441752742879c4c484fd247dd6
