<!-- <template>

    <div class="vm">
        <div class="container" id="clubs">
            <div class="filter">
                <label><input type="checkbox" v-model="selectedCategory" value="All" /> All</label>
                <label><input type="checkbox" v-model="selectedCategory" value="ClubParking" /> Parking</label>
                <label><input type="checkbox" v-model="selectedCategory" value="ClubToilets" /> Toilets</label>
                <label><input type="checkbox" v-model="selectedCategory" value="ClubFloodlights" /> Floodlights</label>
            </div>

            <ul class="clubs-list">
                <li v-for="club in filteredClubs" :key="club">{{ club.clubName }}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data: {
        clubs: [{
            clubName: "Club One",
            clubParking: true,
            clubToilets: false,
            clubFloodlights: true
        },
        {
            clubName: "Club Two",
            clubParking: true,
            clubToilets: false,
            clubFloodlights: false
        },
        {
            clubName: "Club Three",
            clubParking: false,
            clubToilets: true,
            clubFloodlights: true
        },
        ],
        selectedCategory: "All"
    },
    computed: {
        filteredClubs: function () {
            var vm = this;
            var category = vm.selectedCategory;

            if (category === "All") {
                return vm.clubs;
            } else {

                return vm.clubs.filter(function (club) {
                    const selectedFieldNames = selectedCategory.map(category => {
                        switch (category) {
                            case 'Toilets':
                                return 'clubToilets';
                            case 'Parking':
                                return 'clubParking';
                            case 'Floodlights':
                                return 'clubFloodlights';
                        }
                    })

                });



            }
            return vm.clubs.filter(function (club) {
                return selectedFieldNames.every(fname => club[fname])
            }
        }
    }
}
</script>

<style scoped>
h3 {
    margin-bottom: 0;
}

p {
    margin: 0;
}

.options {
    padding-bottom: 1rem;
    border-bottom: 1px solid LightGrey;
}
</style> -->
