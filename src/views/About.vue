<template>
  <h2 class="text-center my-5 text-2xl">
    Medal Rankings for the 2020 Tokyo Olympic Games
  </h2>

  <div class="container mx-auto text-center">
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>Ranking by Gold Medal</h2>
      <h2>Country</h2>
      <img
        class="medal"
        src="../../public/images/gold-medal.png"
        alt="gold-medal"
      />
      <img
        class="medal"
        src="../../public/images/silver-medal.png"
        alt="silver-medal"
      />
      <img
        class="medal"
        src="../../public/images/bronze-medal.png"
        alt="bronze-medal"
      />
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>1</h2>
      <h2>CHINA</h2>
      <h2>34</h2>
      <h2>24</h2>
      <h2>16</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>2</h2>
      <h2>United States</h2>
      <h2>29</h2>
      <h2>35</h2>
      <h2>27</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>3</h2>
      <h2>Japan</h2>
      <h2>22</h2>
      <h2>10</h2>
      <h2>14</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>4</h2>
      <h2>Australia</h2>
      <h2>17</h2>
      <h2>5</h2>
      <h2>19</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>5</h2>
      <h2>ROC</h2>
      <h2>16</h2>
      <h2>22</h2>
      <h2>20</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>6</h2>
      <h2>Great Britain</h2>
      <h2>16</h2>
      <h2>18</h2>
      <h2>17</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>7</h2>
      <h2>Germany</h2>
      <h2>9</h2>
      <h2>10</h2>
      <h2>16</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>8</h2>
      <h2>France</h2>
      <h2>7</h2>
      <h2>11</h2>
      <h2>9</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>9</h2>
      <h2>Italy</h2>
      <h2>7</h2>
      <h2>10</h2>
      <h2>18</h2>
    </div>
    <div class="form-line grid grid-cols-5 gap-4">
      <h2>10</h2>
      <h2>New Zealand</h2>
      <h2>7</h2>
      <h2>6</h2>
      <h2>6</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "rankings",
};
</script>

<style>
.form-line {
  border: 1px solid black;
  padding: 0.5em;
}
.medal {
  width: 2em;
  display: block;
  margin: 0 auto;
}
</style>
