 [v0.0.8](https://github.com/littleflute/a26/edit/master/README.md)

[SRV Disc 1](SRV Disc 1/)

<audio controls id="player"> 
  <source src="https://littleflute.github.io/a26/cd1/01 Track 1.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
<div id="xd"> 
</div>
<script>
var d = document.getElementById("xd"); 
var html = d.innerHTML; 
html += " a2<br>cd1<br>CD:<br>";
for(var n=1; n<=19; n++)
{	
 	html += fNewBtn(n);

} 
d.innerHTML = html;

var p = document.getElementById("player");
function f(i)
{
    var s = "https://littleflute.github.io/a26/cd1/";
    if(i==111)
    {
        s += "01 Thunderbird.mp3";
    } 
    else
    {
        if(i<10) 
        {
    	    s += "0";
        } 
        s += i;
        s += " Track ";
        s += i;
        s += ".mp3";
    }
	p.src = s; 
    p.play();
}
function fNewBtn(i)
{
	var rHTML = "";
    rHTML = "<button onclick='f(";
    rHTML += i;
    rHTML += ");'>";
    rHTML += i;
    rHTML += "</button>";
    return rHTML;
}
</script>






