# GTA-return-address-spoofing
works with most public invokers, spoofs the return address to act as a bypass and allow checked natives to be called.

Implement in your invoker EndCall example:</br>
`spoof_call(g_GameVariables->GetNativeReturnAddress(), static_cast<void(*)(rage::scrNativeCallContext*)>(handler), static_cast<rage::scrNativeCallContext*>(&m_Context));`
