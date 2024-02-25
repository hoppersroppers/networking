# Scripting and tshark

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/npk0BDqaU1Q?wmode=opaque" width="640"></iframe>  

Even better than viewing packets in a GUI is playing with them using a
scripting language. We're hackers, so we are supposed to use the CLI
(honestly though, Wireshark is better for like... 99% of all situations
that don't involve CLI only access or insanely large pcaps). The tool of
choice for this is named tshark. 

tShark is a command line tool to do the same things that Wireshark does,
but all in python. It is pretty awesome and allows you to script complex
activities that you could never do in Wireshark. 

Follow this tutorial:
<a href="https://hackertarget.com/tshark-tutorial-and-filter-examples/"
rel="noopener"
target="_blank">https://hackertarget.com/tshark-tutorial-and-filter-examples/</a>

To create your initial pcap, run the command "tshark -i wlan0 -w
capture-output.pcap" and then visit
<a href="https://hoppersroppers.org/" rel="noopener"
target="_blank">https://hoppersroppers.org</a> and <http://zombo.com/>.
Then stop the capture with a ctrl-c. 

Afterwards continue through the rest of the tutorial using the pcap you
recorded.
