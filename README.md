# Gnat
Crazy small css flex framework.

## Small, Kind, and Malleable
Gnat was made to handle responsive flex based layouts in a simple and flexible manner which plays well with your own stylesheet. Thanks to CSS's rem unit, Gnat's padding and margins are easily customized by setting the "font-size" on the "html" element. 

Gnat assumes you prototype your layout, and then lay your styling on top of it. If you don't like the silouhette of something, there's no point in dressing it up. 

*By default 1rem = 10px.*

The API is as follows:
```
.pad, .flex { padding:1.25rem; }
.flex { justify-content:space-around;display:flex; }
.col { flex-direction:column; }
.mrg { margin:1.25rem; }
.auto { margin:auto; }
.fill { margin:-1.25rem; }

.one {flex-grow:1;}
.two {flex-grow:2;}
.three {flex-grow:3;}
.four {flex-grow:4;}
.five {flex-grow:5;}
.six {flex-grow:6;}
.seven {flex-grow:7}
.eight {flex-grow:8}
.nine {flex-grow:9}
.ten {flex-grow:10}
.eleven {flex-grow:11}
.twelve {flex-grow:12}

.full {width:calc(100% - 1.25rem);}
.half {width:calc(50% - 1.25rem);}
.third {width:calc(33.33% - 1.25rem);}
.quarter {width:calc(25% - 1.25rem);}
.fith {width:calc(20% - 1.25rem);}
.sixth {width:calc(20% - 1.25rem);}
.seventh {width:calc(20% - 1.25rem);}
.eighth {width:calc(12.5% - 1.25rem);}

.start {align-self:flex-start;}
.center {align-self:center;}
.end {align-self:flex-end;}

@media only screen and (max-width:750px) {
	body, .flex {flex-direction:column;}
	.full, .half, .third, .quarter, .fith, .eigth {width:calc(100% - 1.5rem);height:auto;}
	.end, .center, .start {align-self:stretch;}
}
```

