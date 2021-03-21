<detail>
  <summary>Updating to v0.4.0</summary>
  
  - `answer_str` -> `answer`
  - Don't write `.send()` after each request, now it is done automatically.
  - Use `.auto_send()` to construct your bot: `let bot = Bot::from_env().auto_send();`.
  - `UpdateWithCx<Message>` -> `UpdateWithCx<AutoSend<Bot>, Message>`
  - `ResponseResult<()>` -> `Result<(), Box<dyn Error + Send + Sync>>` (or import `ResponseResult` beforehand: `use teloxide::requests::ResponseResult;`)

</detail>
