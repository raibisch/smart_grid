## Dynamic electricity price with price cap?

"Dynamic electricity prices" ...what is that? ...is that available for me too? ...do I want that? ...opportunities and risks?

# REMARK: This article is primarily relevant for the German market and regulation (Paragraph 14a Regulation EnWg)


### What's that:
Dynamic electricity prices are electricity prices that are usually negotiated as an hourly price the day before on the EPEX electricity exchange. Due to the high proportion of renewable energies, Germany has a very volatile hourly electricity price (including network charges and taxes between 5 and 50 cents). The average electricity price is usually lower (between 15 and 35 cents) than the prices of annual contracts with a price guarantee.

Is that available for me too: From 2025, electricity providers (including for private consumers) must offer at least one dynamic electricity tariff. However, since this requires a digital "smart meter" (= intelligent electricity meter), initially only households with an annual consumption of more than 6000 kW/h and large PV systems (> 7kW peak) will be able to use this tariff (the regulation also mentions households with a "controllable consumption device" (= heat pump or wall box), but I don't know anyone with a heat pump or wall box who has automatically received a different meter. Without this "smart meter", only the electricity provider "Tibber" can currently offer an hourly price for digital electricity meters without a network connection (= modern measuring device) with the help of an adapter, but to be honest, that's more for "electricity nerds".

### Who need this:
A dynamic tariff is interesting for everyone who can shift their electricity consumption (at least partially) to the cheaper hours of the day and night. In private households, this is primarily the consumers of electric cars and heat pumps.

### The opportunities:
First of all, we all benefit from it if our electricity consumption is well adapted to the supply of renewable energies (the grid remains stable and fewer wind turbines have to be throttled down). Charging the electric car can be easily postponed to the cheaper hours (with 20-40kW per day there is also great potential here).

The heat pump can also be operated - at least to a certain extent - in such a way that at least the price peaks can be avoided with the help of the "smart-ready" function of the newer heat pumps.

### The risks:
There is no price guarantee or an automatic "price brake" for the hourly price!... and predictions - especially if they are in the future - are always difficult ;-)

### EPEX (european electric energy exchange) breakdown: On June 26, 2024, electricity customers with dynamic tariffs experienced the electricity price super-accident: Between 6:00 and 7:00 a.m., the prices for one kWh shot up to around 2.30 euros (for one hour on the 22kW wallbox, that's around 50 euros). The reason was a "software error" on the EPEX electricity exchange. To date, there has been no compensation for this, nor have measures been announced to protect consumers from such errors in the future.

### To do or not to do?
It would be nice if you could calculate the costs in advance "virtually" using a simulation based on the consumption profile (and then make a sensible and fact-based decision).
If you ultimately want to use this, a built-in "price brake" (see EPEX glitch) would be desirable, which regulates the wall box and heat pump down when electricity prices are very high.
It would be even better, of course, to optimize the consumption of the wall box and heat pump depending on the electricity price and possibly include a PV system.
...too much to ask for?
I've now made a start and put together a 5-10€ solution for all software and electronics nerds (which, as always, is open source and freely available)

#### What's already possible:
- Determining the current hourly electricity prices (including all taxes and network charges!)
- Display of the data on a web app (for all mobile devices and PCs)
- Rule-based evaluation (for controlling heat pumps or wall boxes)
- SmartGrid-ready control (relay output) for all SG-ready heat pumps
- Much more (Modbus for external electricity meters, logging of data from AIT heat pumps)
#### What's coming soon:
- "virtual" electricity bill (in conjunction with a reader for digital electricity meters)
- Modbus control for wall boxes (currently only planned for ABL wall boxes)
