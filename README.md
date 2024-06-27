# Diler-kendaraan
class Kendaraan:
    def __init__(self, model, harga):
        self.model = model
        self.harga = harga

class Dealer:
    def __init__(self):
        self.kendaraan_list = []

    def tambah_kendaraan(self, kendaraan):
        self.kendaraan_list.append(kendaraan)

if __name__ == '__main__':
    dealer = Dealer()
    kendaraan1 = Kendaraan('Toyota', 200000000)
    kendaraan2 = Kendaraan('Honda', 180000000)
    dealer.tambah_kendaraan(kendaraan1)
    dealer.tambah_kendaraan(kendaraan2)
    print(f'Kendaraan yang tersedia: {[k.model for k in dealer.kendaraan_list]}')
    
