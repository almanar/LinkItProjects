This example connects to HTTP(not HTTPS) to retrieve index.html from labs.mediatek.com and print to vm_log.

It calls the API vm_https_register_context_and_callback() to register the callback functions, then set the channel by vm_https_set_channel(). After the channel is established, it will send out the request by vm_https_send_request() and read the response by vm_https_read_content().

You can change the url by modify macro VMHTTPS_TEST_URL.
Before run this example, please set the APN information first by modify macros.